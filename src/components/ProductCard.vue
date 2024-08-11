<template>
    <div class="col-md-4 mb-4">
      <div class="card">
        <img :src="product.image" class="card-img-top" :alt="product.name">
        <div class="card-body">
          <h5 class="card-title">{{ product.name }}</h5>
          <p class="card-text">{{ product.description }}</p>
          <p class="card-text"><strong>Precio: ${{ product.price }}</strong></p>
          <button @click="addToCart" class="btn btn-primary">Agregar al carrito</button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProductCard',
    props: ['product'],
    methods: {
      addToCart() {
        // Implementar lógica para agregar al carrito
        console.log('Producto agregado:', this.product);
      }
    }
  }
  </script>