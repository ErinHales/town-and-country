<script setup>
// import { ref } from 'vue'

// defineProps({
//   msg: String
// })

// const count = ref(0)
</script>

<template>
  <div class="nav">
    <div class="nav-container">
      <img src="../assets/TC-logo.png" class="logo" />
      <div class="nav__right">
        <a href="">Claim</a>
        <img src="../assets/menu.svg" class="menu" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.nav {
  background-color: #1465AE;
  height: 50px;
  padding: 10px 40px;
  display: flex;
  justify-content: center;
}
.nav-container {
  width: 100%;
  max-width: 1200px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.logo {
  height: 100%;
}
.nav__right {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.menu {
  height: 100%;
  margin-left: 20px;
}
</style>