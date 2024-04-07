<script setup>
// import { ref } from 'vue'
// const routes = ref([
// {id:'1', to: '/', title: 'Home' }, 
// {id:'2',  to: 'features', title: 'Features' }, 
// {id:'3', to: 'policy', title: 'Privacy policy' }, 
// {id:'4',  to: 'req-feature', title: 'Request Feature' },]) 
const props = defineProps({
    card: Object
})
</script>

<template>
    <nuxt-link class="link" :to=card.link >
        <article class="article">
            <NuxtImg class="image" width="370px" height="195px" :src=card.cardImg />
            <h3 class="title">{{ card.title }}</h3>
            <p class="text">{{ card.text }}</p>
            <time class="time" datetime="2024-04-07T14:54">
                <div class="dayWrapper">
                    <CalendarIcon />
                    Today
                </div>
                <CircleIcon />
                <div class="minutsWrapper">
                    13m ago</div>
            </time>
        </article>
    </nuxt-link>
</template>

<style scoped>
.link {
    all: unset;
    cursor: pointer;
}

.article {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.title {
    margin: 0;
    padding: 0;
    color: var(--text-card-title);
    font-family: var(--font-family);
    font-weight: 500;
    font-size: 22px;
    line-height: 150%;

    text-align: left;
}

.text {
    margin: 0;
    padding: 0;
    font-family: var(--font-family);
    font-weight: 400;
    font-size: 16px;
    line-height: 170%;
    color: var(--text-color-white);
    text-align: left;
}

.time {
    font-family: var(--font-family);
    font-weight: 300;
    font-size: 16px;
    line-height: 100%;
    color: var(--text-card-time-gray);
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 10px;
    padding-top: 10px;
}

.dayWrapper {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 5px;
}
</style>
