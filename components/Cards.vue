<script setup>

const cardsArray = [{
    id: 1,
    title: "Sit curabitur cum dolor mauris",
    text: "Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada tincidunt enim auctor",
    time: "2024-04-07T14:54",
    link: `/1-card`,
    cardImg: "/card1.png"
},
{
    id: 2,
    title: "Lorem ipsum dolor sit ametconsectetur. Auctor at cursus amet aliquet gravida",
    text: "Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada",
    time: "2024-04-07T14:54",
    link: `/2-card`,
    cardImg: "/card2.png"
},
{
    id: 3,
    title: "Sit curabitur cum dolor mauris augue massa",
    text: "Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada tincidunt enim auctor",
    time: "2024-04-07T14:54",
    link: `/3-card`,
    cardImg: "/card1.png"
},
{
    id: 4,
    title: "Lorem ipsum dolor sit amet con...",
    text: "Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada ",
    time: "2024-04-07T14:54",
    link: `/4-card`,
    cardImg: "/card2.png"
},
{
    id: 5,
    title: "Sit curabitur cum dolor mauris",
    text: "Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada tincidunt enim auctor",
    time: "2024-04-07T14:54",
    link: `/5-card`,
    cardImg: "/card1.png"
},
{
    id: 6,
    title: "Sit curabitur cum dolor mauris",
    text: "Sit curabitur cum dolor mauris. Sit augue massa diam donec consequat malesuada tincidunt enim auctor",
    time: "2024-04-07T14:54",
    link: `/6-card`,
    cardImg: "/card3.png"
},
]
</script>

<template>
    <section class="section">
        <MainCard />
        <SecondaryCard v-for="card in cardsArray" :card="card" :key="card.id" />
    </section>
</template>

<style scoped>
.section {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
    grid-template-areas:
        "mainCard mainCard mainCard"
        "card card card"
        "card card card";
    gap: 35px;
    width: 100%;
    max-width: 1440px;
    box-sizing: border-box;
    padding: 50px 132px 345px;
    margin: 0 auto;

}

div {
    width: 100%;
    min-height: 300px;
}
</style>
