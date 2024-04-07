<script>
</script>

<template>
    <header class="header">
        <Logo />
        <div class="rightSideWrapper">
            <Navbar />
            <button class="button">Download</button>
        </div>
    </header>
</template>

<style scoped>
.header {
    position: absolute;
    top: 0;
    left: calc((100dvw - 1440px) / 2);
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    height: 100px;
    padding: 0 132px;
    width: 100%;
    max-width: 1440px;
    box-sizing: border-box;
    margin: 0 auto;
    backdrop-filter: blur(20px);
    background: rgba(9, 5, 22, 0.15);
    z-index: var(--header-layer);
}

.button {
    all:unset;
    cursor: pointer;
    font-family: var(--second-family);
    font-weight: 500;
    font-size: 14px;
    text-align: center;
    color: var(--text-color-white);
    width: 122px;
    height: 40px;
    border: 1px solid var(--text-color-white);
    border-radius: 40px;
    box-sizing: border-box;
}

.rightSideWrapper {
    display: flex;
    flex-direction: row;
    gap: 68px;
}

</style>
