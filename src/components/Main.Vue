<script>
import productCard from '../data/productCard'

  export default {
    name: 'Main',
    data(){
      return {
        productCard
      }
    }
  }
</script>

<template>
  <main>
    <section class="container flex cards">

      <div class="product"
      v-for="(product, index) in productCard"
      :key="index"
      >
        <div class="trasp">
          <!-- modello -->
          <img class="model part" 
          :src="`/img/${product.primaryImage}`" 
          :alt="primaryImage">
          
          <img class="model view" 
          :src="`/img/${product.secondaryImage}`" 
          :alt="secondaryImage">
          <span class="heart">&hearts;</span>
          <!-- /modello -->
      
        
          <div class="label">
            <span class="sale">{{product.discount}}</span>
            <span class="eco"
            v-if="(product.sostenibilita === false) ? 'hide' : ''">
            Sostenibilità
            </span>
          </div>
        </div>

        <div class="info">
          <span class="brand">Levi's</span>
          <h3
          class="title">Relaxed fit tee unisex </h3>
          <span class="price-special">14,99&euro;</span>
          <span class="price">29,99 &euro;</span>
        </div>       
      </div>

    </section>
  </main>

</template>

<style lang="scss">
  @use '../scss/main.scss';
</style>

