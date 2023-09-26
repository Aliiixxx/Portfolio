<template>
  <div>
    <modale :revele="revele" :toggleModale="toggleModale"></modale>
    <Button label="Primary" v-on:click="toggleModale" class="btn btn-success"
      >Plus d'infos</Button
    >
  </div>
</template>

<script>
import Modale from "./MondalCahier.vue";

export default {
  name: "ContenuCahier",
  data() {
    return {
      revele: false,
    };
  },
  components: {
    modale: Modale,
  },
  methods: {
    toggleModale: function () {
      this.revele = !this.revele;
    },
  },
};
</script>

<style></style>
