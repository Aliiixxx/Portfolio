<template>
  <div class="container">
    <form @submit.prevent="submit">
      <div class="form-group">
        <label for="nom">Nom</label>
        <input type="text" class="form-control" id="nom" v-model="nom" />
      </div>
      <div class="form-group">
        <label for="prenom">Prénom</label>
        <input type="text" class="form-control" id="prenom" v-model="prenom" />
      </div>
      <div class="form-group">
        <label for="objet">Objet</label>
        <input type="text" class="form-control" id="objet" v-model="objet" />
      </div>
      <div class="form-group">
        <label for="message">Message</label>
        <textarea
          class="form-control"
          id="message"
          v-model="message"
        ></textarea>
      </div>
      <button type="submit" class="btn btn-primary">Envoyer</button>
    </form>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "ContactForm",
  data() {
    return {
      nom: "",
      prenom: "",
      objet: "",
      message: "",
    };
  },
  methods: {
    submit() {
      if (!this.nom || !this.prenom || !this.objet || !this.message) {
        alert("Veuillez remplir tous les champs requis.");
        return;
      }
      alert("Votre message a été envoyé a Verrier_alix@hotmail.fr.");
    },
  },
});
</script>

<style>
.form-group textarea {
  width: 300px;
  height: 64px;
}
</style>
