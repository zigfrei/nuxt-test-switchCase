<script setup>
const topCard = {
    title: "Lorem ipsum dolor sit amet consectetur",
    text: "Lorem ipsum dolor sit amet consectetur. Auctor at cursus amet aliquet gravida condimentum tortor. Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada tincidunt enim auctor. Sit augue massa diam donec",
    time: "2024-04-07T14:54",
    link: "/main-card"
}
</script>

<template>
    <nuxt-link class="link" :to=topCard.link>
        <div class=" textWrapper">
        <h3 class="title">{{ topCard.title }}</h3>
        <p class="text">{{ topCard.text }}</p>
        <time class="time" datetime="2024-04-07T14:54">
            <div class="dayWrapper">
                <CalendarIcon />
                Today
            </div>
            <CircleIcon />
            <div class="minutsWrapper">
                13m ago</div>
        </time>
        </div>
        <NuxtImg class="image" width="775px" height="315px" src="/topNewsImage.png" />
    </nuxt-link>
</template>

<style scoped>
.link {
    all: unset;
    cursor: pointer;
    grid-area: mainCard;
    display: grid;
    grid-column: span 3 / 4;
    grid-row: 1 / 2;
    grid-template-columns: subgrid;
    grid-template-rows: subgrid;
    grid-template-areas:
        "mainCardText mainCardImg mainCardImg";
    align-items: center;

}

.textWrapper {
    grid-area: mainCardText;
    display: flex;
    flex-direction: column;
    gap: 17px;
    width: 367px;
}

.image {
    grid-area: mainCardImg;
}

.title {
    margin: 0;
    padding: 0;
    font-family: var(--font-family);
    font-weight: 500;
    font-size: 35px;
    line-height: 150%;
    background: linear-gradient(88deg, #fff 0%, #664ff3 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
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
