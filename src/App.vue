<template>
  <div id="app">
    <Navigation />

    <router-view />
    <footer id="footer">
      footer
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
