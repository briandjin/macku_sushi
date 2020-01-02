<template>
  <div id="app">
    <Navigation />

    <router-view />
    <footer id="footer">
      <div class="address__container">
        <p class="address">2239 N CLYBOURN AVE.</p>
        <a href="tel:(773)880-8012">773.880.8012</a>
      </div>
      <div class="icons">
        <img src="https://static.wixstatic.com/media/e1a85976534f42c1a09d3bff23646ba2.png" alt="">
        <img src="https://static.wixstatic.com/media/e1a85976534f42c1a09d3bff23646ba2.png" alt="">
        <img src="https://static.wixstatic.com/media/e1a85976534f42c1a09d3bff23646ba2.png" alt="">
      </div>
    </footer>
  </div>
</template>

<script>
import Navigation from '@/components/Navigation/index.vue';

export default {
  name: 'App',
  components: {
    Navigation,
  },
};
</script>

<style lang="scss" src="./styles/index.scss"></style>
