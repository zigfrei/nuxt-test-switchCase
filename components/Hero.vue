<script>
</script>

<template>
    <section class="section">
        <div class="contentWrapper">
            <NuxtImg width="373px" height="298px" src="/imgBlog.png" />
            <h2 class="title">Blog</h2>
            <img class="imageBG" src="../public/imgBlogBG.png">
        </div>
        <img class="bgLeft" src="../public/imgHerobg1.png">
        <img class="bgMiddle" src="../public/imgHerobg2.png">
        <img class="bgRight" src="../public/imgHerobg3.png">
    </section>
</template>

<style scoped>
.section {
    position: relative;
    padding: 139px 0 88px 0;
    display: flex;
    justify-content: center;
    box-sizing: border-box;
    box-shadow: 0 20px 100px 0 rgba(121, 88, 252, 0.2);
    background: #020203, radial-gradient(55.48% 58.17% at 101.46% 32.19%, rgb(2, 80, 24) 0%, rgb(2, 80, 24) 100%), radial-gradient(120.83% 69.48% at 84.3% 2.48%, rgb(80, 2, 50) 0%, rgb(79, 3, 49) 100%);
}

.contentWrapper {
    position: relative;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 68px;
}

.title {
    margin: 0;
    padding: 20px 0 0;
    font-family: var(--font-family);
    font-weight: 600;
    font-size: 70px;
    line-height: 143%;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--text-color-white);

}

.imageBG {
    position: absolute;
    top: -140px;
    left: -170px;
    z-index: -1;
}

.bgLeft {
    position: absolute;
    top: 84px;
    left: -65px;
    z-index: var(--decoration-layer);
}

.bgMiddle {
    position: absolute;
    top: 117px;
    left: 906px;
    z-index: var(--decoration-layer);
}

.bgRight {
    position: absolute;
    top: 28px;
    right: -7px;
    z-index: var(--decoration-layer);
}
</style>
