<script>
import Nav from './components/Nav.vue';
import Header from './components/Header.vue';
import Banner from './components/Banner.vue';

export default {
  components: {
    Nav,
    Header,
    Banner
  }
}
</script>

<template>
  <Nav />
  <Header />
  <Banner />
</template>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
