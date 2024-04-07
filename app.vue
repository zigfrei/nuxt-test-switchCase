<template>
  <div class="page">
    <Header />
    <main>
      <Hero />
      <Cards />
    </main>
  </div>
  <div class="noise" />
</template>

<style >
.page {
  position: relative;
}

:root{
  
  --font-family: "Poppins", sans-serif;
  --second-family: "Euclid Circular A", sans-serif;
  --third-family: "Actor", sans-serif;

  --text-color-white: #fff;
  --text-color-gray-navbar: #948ea1;
  --text-color-gray-navbar-active: #a073ff;
  --text-card-time-gray: #8f8e9e;
  --text-card-title: #afaedf;

  --decoration-layer: 2;
  --header-layer: 3;
}

body {
  margin: 0 auto;
  width: 100%;
  max-width: 1920px;
  box-sizing: border-box;
  overflow-x: hidden;
}

html {
  position: relative;
  background-color: #000;
}

.noise {
  pointer-events: none;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('/noise-light.png');
  box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.25);
  opacity: 0.3;
}
</style>
