<script setup>
import Dental from '../assets/product-dental.png'
import Vision from '../assets/product-vision.png'
import Annuity from '../assets/product-annuity.png'

const products = [{
  img: Dental,
  title: 'Dental'
}, {
  img: Vision,
  title: 'Vision'
}, {
  img: Annuity,
  title: 'Annuity'
}]
</script>

<template>
  <div class="products">
    <div v-for="(p, i) in products" :key="i" class="product">
      <img :src="p.img" class="product-img" />
      <div>
        <h2 class="product-title">{{ p.title }}</h2>
        <!-- <p>{{ p.description }}</p> -->
      </div>
    </div>
  </div>
</template>

<style>
.products {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 50px 20px;
}
.product {
  display: flex;
  width: 100%;
  max-width: 800px;
  margin: 20px;
  padding: 20px;
  border: 0.5px solid #CECECE;
  border-radius: 10px;
  box-shadow: 0 4px 4px #B0B0B0;
}
.product-title {
  border-bottom: 3px solid #1465AE;
}
.product-img {
  max-height: 100%;
  margin-right: 20px;
}

@media (max-width: 650px) {
  .product {
    flex-direction: column;
  }
}
</style>
