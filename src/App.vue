<script>
  import Header from './components/Header.Vue';
  import Main from './components/Main.Vue';
  import Footer from './components/Footer.Vue';
  
  export default {
  name : 'App',
  components : { Header,
    Main,
    Footer 
  }
}
</script>

<template>
  <Header />
  <Main />
  <Footer />
</template>

<style lang="scss">
  @use './scss/general/general.scss'
</style>