<script>
  import{clientMenu, iconMenu} from '../data/headerMenu'

  export default {
    name: 'Header',
    data() {
      return{
        clientMenu,
        iconMenu
      }
    }
  }
</script>

<template>
  <header class="position">

    <div class="container flex">
      <!-- menu left-->
      <ul class="menu">
        <li 
        v-for="(client, index) in clientMenu"
        :key="index">
          <a :href="client.href">{{client.person}}</a> 
        </li>
      </ul>

      <!-- logo -->
      <img id="logo" src="/img/boolean-logo.png" alt="logo">

      <!-- menu right -->
      <ul class="menu">
        <li v-for="(icon, index) in iconMenu"
        :key="index"><a :href="icon.href"><i :class="icon.icon"></i></a></li>

      </ul>
    </div>

  </header>
</template>


<style lang="scss" scoped>
  @use '../scss/header.scss' as *;

</style>