<template>
  <div class="not-found">
    <img src="../assets/404Image.png" alt="Page introuvable" />
    <p>La page que vous recherchez est introuvable.</p>
    <router-link to="/">Revenir à la page d'accueil</router-link>
  </div>
</template>

<script>
export default {
  name: "NotFound",
};
</script>

<style scoped>
@import "../assets/Styles.css";
.not-found {
  text-align: center;
  padding: 20px;
}

.not-found img {
  max-width: 100%;
  height: auto;
}

.not-found h1 {
  font-size: 2em;
}

.not-found p {
  font-size: 1.2em;
}

.not-found router-link {
  font-size: 1.2em;
}
</style>
