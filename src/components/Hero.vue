<template>
  <div class="hero">
    <img src="../assets/Town&Country.png" class="text" />
  </div>
</template>

<style scoped>
.hero {
  width: 100vw;
  height: calc(100vh - 50px);
  background-image: url('../assets/hero-img.png');
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}
.text {
  width: 100%;
  max-width: 650px;
  margin-bottom: 100px;
}
</style>