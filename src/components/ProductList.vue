<template>
    <div class="row">
      <ProductCard 
        v-for="product in products" 
        :key="product.id" 
        :product="product" 
      />
    </div>
  </template>
  
  <script>
  import ProductCard from '@/components/ProductCard.vue'
  
  export default {
    name: 'ProductList',
    components: {
      ProductCard
    },
    data() {
      return {
        products: [
          { id: 1, name: 'Producto 1', description: 'Descripción del producto 1', price: 19.99, image: 'https://via.placeholder.com/300' },
          { id: 2, name: 'Producto 2', description: 'Descripción del producto 2', price: 29.99, image: 'https://via.placeholder.com/300' },
          { id: 3, name: 'Producto 3', description: 'Descripción del producto 3', price: 39.99, image: 'https://via.placeholder.com/300' },
        ]
      }
    }
  }
  </script>