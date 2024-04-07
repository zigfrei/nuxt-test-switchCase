<script setup>
const routes = [
{id:'1', to: '/', title: 'Home' }, 
{id:'2',  to: 'features', title: 'Features' }, 
{id:'3', to: 'policy', title: 'Privacy policy' }, 
{id:'4',  to: 'req-feature', title: 'Request Feature' },] 
</script>

<template>
    <nav class="navigation">
        <nuxt-link v-for="elem in routes" class="link" :to="elem.to" :key="elem.id">
            {{ elem.title }}
        </nuxt-link>
    </nav>
</template>

<style scoped>
.navigation {
    display: flex;
    flex-direction: row;
    gap: 80px;
}

.link {
    all: unset;
    margin: 0;
    padding: 0;
    font-style: normal;
    font-weight: 300;
    font-size: 16px;
    line-height: 170%;
    text-transform: capitalize;
    font-family: var(--second-family);
    color: var(--text-color-gray-navbar);   
    cursor: pointer;
    display: flex;
    align-items: center;
}

.router-link-active {
font-weight: 400;
color: var(--text-color-gray-navbar-active);
}

.router-link-active::before {
    content: "[ ";
}

.router-link-active::after {
    content: " ]";
}


</style>
