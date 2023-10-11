<script>
  export default {
    name: 'Header'
  }
</script>

<template>
  <header class="position">

    <div class="container flex">
      <!-- menu left-->
      <ul class="menu">
        <li><a href="#">Donna</a></li>
        <li><a href="#">Uomo</a></li>
        <li><a href="#">Bambini</a></li>
      </ul>

      <!-- logo -->
      <img id="logo" src="/img/boolean-logo.png" alt="logo">

      <!-- menu right -->
      <ul class="menu">
        <li><a href="#"><i class="fa-regular fa-user"></i></a></li>
        <li><a href="#"><i class="fa-regular fa-heart"></i></a></li>
        <li><a href="#"><i class="fa-solid fa-bag-shopping"></i></a></li>
      </ul>
    </div>

  </header>
</template>

<style>

</style>

