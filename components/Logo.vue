<script>
</script>

<template>
    <nuxt-link class="link" to="/">
        <div class="logoWrapper">
            <LogoIcon/>
            <h1 class="logoTitle">Sinum</h1>
        </div>
    </nuxt-link>
</template>

<style scoped>
.logoWrapper {
    display: flex;
    flex-direction: row;
    gap: 15px;
}

.logoTitle {
    margin: 0;
    padding: 0;
    font-style: normal;
    color: var(--text-color-white);
    font-weight: 400;
    font-size: 27px;
    line-height: 170%;
    text-transform: capitalize;
    font-family: var(--third-family);
}

.link {
    all: unset;
    cursor: pointer;
}
</style>
