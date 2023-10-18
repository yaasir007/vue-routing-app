<script setup>
import { ref } from 'vue';
import carsData from '../components/data.json'

const cars = ref(carsData);
</script>

<template>
  <main class="container">
    <h1>Cars</h1>
    <div class="cards">
      <div v-for="car in cars" class="card">
        <h2>{{  car.make }}</h2>
        <p>${{ car.price }}</p>
      </div>
    </div>
  </main>
</template>

<style scoped>
.cards {
  width: 100%;
  display: flex;
  justify-content: center;
  align-content: center;
  gap: 1rem;
  flex-wrap: wrap;
}
.card {
  border: 1px solid pink;
}
</style>
