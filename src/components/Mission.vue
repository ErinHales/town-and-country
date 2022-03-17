<script setup>
import Lock from '../assets/lock.svg'
import Equality from '../assets/equality.svg'
import Honesty from '../assets/honesty.svg'
const values = [{
  icon: Lock,
  description: 'Security'
}, {
  icon: Equality,
  description: 'Equality'
}, {
  icon: Honesty,
  description: 'Honesty'
}]
</script>

<template>
  <div class="mission">
    <div class="mission-container">
      <h2 class="mission-title">Our Mission</h2>
      <div class="value-bubbles">
        <div v-for="(v, i) in values" :key="i" class="bubble">
          <img :src="v.icon" class="bubble-icon" />
          <p class="value-bubbles__title">{{ v.description }}</p>
        </div>
      </div>
      <div class="statement">
        <h3>Our mission at Town & Country Life Insurance is providing peace of mind and security through innovative life and health products since 1955.</h3>
      </div>
    </div>
  </div>
</template>

<style>
.mission {
  display: flex;
  justify-content: center;
  background-color: #F5F5F5;
  padding: 60px 40px;
}
.mission-container {
  width: 100%;
  max-width: 800px;
}
.mission-title {
  margin-left: 20px;
  margin-bottom: 40px;
}
.value-bubbles {
  display: flex;
  justify-content: space-between;
}
.value-bubbles__title {
  font-size: 20px;
}
.bubble {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  margin: 10px;
  background-color: #1465AE;
  box-shadow: 0 4px 4px #B0B0B0;
}
.bubble-icon {
  height: 56px;
}
.statement {
  text-align: center;
  max-width: 400px;
  font-size: 18px;
  line-height: 2.5;
  margin: 100px auto 50px auto;
}

@media (max-width: 700px) {
  .value-bubbles {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .bubble {
    margin-bottom: 20px;
  }
}
</style>
