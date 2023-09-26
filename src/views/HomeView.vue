<template>
  <section id="presentation">
    <h1 id="fullname">Verrier Alix</h1>
    <p>
      Je suis un développeur web en herbe,je suis passionné par le développement
      web depuis le début de ma formation. J'ai toujours été intéressé par les
      nouvelles technologies et j'ai trouvé dans le développement web un moyen
      de les mettre en pratique.
    </p>
    <p>
      J'apprécie le challenge de créer des sites web fonctionnels et
      esthétiques. J'aime également apprendre de nouvelles choses et je suis
      toujours à la recherche de nouvelles technologies à explorer.
    </p>
    <p>
      Dans mon portfolio, vous trouverez une sélection de mes projets les plus
      récents. J'espère que vous les apprécierez.
    </p>
  </section>
  <section id="creations">
    <h1 id="ProjetTitre">Mes créations</h1>
    <ul id="liste">
      <li id="cv">
        Curriculum Vitae:
        <contenuCv />
        <img src="../assets/ImageCv.PNG" alt="ImageCv" id="Imageprjet" />
      </li>
      <li id="Cahier">
        Cahier des charges:
        <contenuCahier />
        <Carrousel id="Carrousel" />
      </li>
      <li id="Dynamiser">
        Dynamiser un espace de commentaires:
        <contenuDynamiser />
        <img src="../assets/ImageDynamiser.PNG" alt="ImageCv" id="Imageprjet" />
      </li>
    </ul>
  </section>
  <section id="ContactTitre">
    <h1>Contactez–moi</h1>
    <contact-form></contact-form>
  </section>
</template>

<style>
@import "../assets/Styles.css";
</style>

<script>
import ContenuDynamiser from "../components/ContenuDynamiser.vue";
import ContenuCahier from "../components/ContenuCahier.vue";
import ContenuCv from "../components/ContenuCv.vue";
import ContactForm from "../components/ContactForm.vue";
import Carrousel from "../components/Carrousel.vue";

export default {
  name: "Home",
  components: {
    contenuDynamiser: ContenuDynamiser,
    contenuCahier: ContenuCahier,
    contenuCv: ContenuCv,
    contactForm: ContactForm,
    Carrousel,
  },
};
</script>
