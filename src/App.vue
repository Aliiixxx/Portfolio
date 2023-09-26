<template>
  <div id="app">
    <header>
      <HeaderApp></HeaderApp>
    </header>
    <main id="MainApp">
      <RouterView></RouterView>
    </main>
    <footer>
      <FooterApp></FooterApp>
      <back-to-top></back-to-top>
    </footer>
  </div>
</template>

<script>
import { RouterLink, RouterView } from "vue-router";
import BackToTop from "./components/BackToTop.vue";
import Home from "./views/HomeView.vue";
import HeaderApp from "./views/Header.vue";
import FooterApp from "./views/Footer.vue";

export default {
  name: "components",
  components: {
    BackToTop,
    HeaderApp,
    FooterApp,
    Home,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lato&family=Raleway&family=Roboto&display=swap");
@import "./assets/Styles.css";
</style>
