<template>
  <div id="HeaderColor">
    <nav>
      <RouterLink to="/">
        <img src="../../src/assets/IconHome.png" alt="Image" id="ImageHome" />
      </RouterLink>
      <h1 id="titre">Portfolio</h1>
      <router-link to="/404" id="AutrePage">Autre Page</router-link>

      <Menu />
    </nav>
  </div>
</template>

<script>
import { RouterLink, RouterView } from "vue-router";
import Menu from "../components/Menu.vue";

export default {
  name: "HeaderApp",
  components: {
    Menu,
  },
};
</script>

<style>
@import "../assets/Styles.css";
</style>
