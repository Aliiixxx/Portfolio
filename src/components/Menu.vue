<template>
  <nav id="Menu">
    <a class="nav-link" href="#presentation">Présentation</a>
    <a class="nav-link" href="#creations">Créations</a>
    <a class="nav-link" href="#ContactTitre">Contact</a>
  </nav>
</template>

<script>
export default {
  name: "Menu",
};
</script>

<style scoped>
.nav-link {
  color: #790e3c;
}

#Menu {
  background-color: aliceblue;
  border-radius: 25%;
  height: 110px;
  width: 110px;
  padding: 5px;
  font-size: 18px;
  display: flex;
  flex-direction: column;
}
</style>
