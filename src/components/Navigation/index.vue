<template>
  <div id="nav">
    <transition name="flip">
      <div class="nav-btn__wrapper" v-show="showMobileMenu">
        <router-link class="nav__btn" to="/">HOME</router-link>
        <router-link class="nav__btn" to="/about">MENU</router-link>
        <a
          target="_blank"
          class="nav__btn"
          href="https://ordering.chownow.com/order/4388/locations"
        >
          ONLINE ORDERING
        </a>
        <router-link class="nav__btn" to="/about">WHISKY</router-link>
        <router-link class="nav__btn" to="/about">GALLERY</router-link>
        <router-link class="nav__btn" to="/about">PRESS</router-link>
      </div>
    </transition>
    <!-- eslint-disable  -->

    <svg
      class="ham hamRotate ham4"
      viewBox="0 0 100 100"
      width="60"
      ref="ham"
      @click="handleHamMenuClick"
    >
      <path
        class="line top"
        d="m 70,33 h -40 c 0,0 -8.5,-0.149796 -8.5,8.5 0,8.649796 8.5,8.5 8.5,8.5 h 20 v -20"
      />
      <path class="line middle" d="m 70,50 h -40" />
      <path
        class="line bottom"
        d="m 30,67 h 40 c 0,0 8.5,0.149796 8.5,-8.5 0,-8.649796 -8.5,-8.5 -8.5,-8.5 h -20 v 20"
      />
    </svg>
    <!-- eslint-enable  -->
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  data() {
    return {
      showMobileMenu: false,
    };
  },
  methods: {
    handleHamMenuClick() {
      this.$refs.ham.classList.toggle('active');
      this.showMobileMenu = !this.showMobileMenu;
    },
  },
};
</script>

<style lang="scss" src="./index.scss"></style>
