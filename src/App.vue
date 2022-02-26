<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Nav from './components/Nav.vue'
import HeroImg from './components/Hero.vue'
import Products from './components/Products.vue'
import Mission from './components/Mission.vue'
import Contact from './components/Contact.vue'
</script>

<template>
  <Nav />
  <HeroImg />
  <Products />
  <Mission />
  <Contact />
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&family=Prata&display=swap');

* {
  box-sizing: border-box;
}
body {
  margin: 0;
  font-family: 'Montserrat', sans-serif;
}
h1, h2 {
  font-family: 'Prata', serif;
}
a {
  color: #fff;
  text-decoration: none;
}
</style>
