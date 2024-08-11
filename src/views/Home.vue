<template>
    <div class="container mt-4">
      <h1 class="text-center mb-4">Bienvenido a nuestra tienda</h1>
      <ProductList />
    </div>
  </template>
  
  <script>
  import ProductList from '@/components/ProductList.vue'
  
  export default {
    name: 'HomePage',
    components: {
      ProductList
    }
  }
  </script>