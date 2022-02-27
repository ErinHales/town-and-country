<script setup>
const values = [{
  icon: '../assets/menu.svg',
  description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit'
}, {
  icon: '../assets/menu.svg',
  description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit'
}, {
  icon: '../assets/menu.svg',
  description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit'
}]
</script>

<template>
  <div class="mission">
    <div class="mission-container">
      <h2 class="mission-title">Our Mission</h2>
      <div class="value-bubbles">
        <div v-for="(v, i) in values" :key="i" class="bubble">
          <img src="../assets/lock.svg" class="bubble-icon" />
          <p>{{ v.description }}</p>
        </div>
      </div>
      <div class="statement">
        <h3>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In lorem risus, eleifend ac quam ac, congue mattis neque.</h3>
        <h3>Aenean nunc risus, posuere non hendrerit quis, dictum sit amet quam. Suspendisse tempus purus volutpat, tempus turpis at, pellentesque ex.</h3>
        <h3>Nulla pulvinar ornare dolor. Vestibulum quis augue ut mi auctor rhoncus. Pellentesque justo tellus, egestas efficitur congue tempus, congue ac turpis. Nullam semper nulla vitae commodo pretium. Etiam nec sapien enim. Vestibulum magna ligula, rhoncus in imperdiet sit amet, accumsan sed risus. Fusce sed suscipit libero.</h3>
        <h3>Curabitur finibus ac dolor et posuere. Nulla facilisi. Nulla facilisi. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</h3>
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
  margin-top: 50px;
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
