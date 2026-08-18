<template>
  <div class="products-page">
    <h1>芋小宝甜品商城</h1>
    <p>精选东方甜品与限定礼盒</p>
    <div class="products">
      <div v-for="item in products" :key="item.name" class="card">
        <h3>{{ item.name }}</h3>
        <p>{{ item.description }}</p>
        <strong>¥{{ item.price }}</strong>
      </div>
    </div>
  </div>
</template>

<script setup>
import { products } from '../data/products'
</script>
