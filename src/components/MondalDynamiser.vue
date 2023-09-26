<template>
  <div class="bloc-modale" v-if="revele">
    <div class="overlay" v-on:click="toggleModale"></div>

    <div class="modale card">
      <Button
        label="Submit"
        v-on:click="toggleModale"
        class="btn-modale btn btn-danger"
        >X</Button
      >
      <h2>Curriculum Vitae</h2>
      <ul>
        <li>Fais le <time datetime="2023-09-14">14 septembre 2023</time></li>
        <li>Technologies utilisées : HTML/CSS/JavaScript</li>
        <li>
          Lien vers le repository :
          <a
            href="https://github.com/Aliiixxx/DynamiserUnEspaceDeCommentaires_DocumentsDevoir"
            target="_blank"
            >Github</a
          >
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "ModaleContact",
  props: ["revele", "toggleModale"],
};
</script>

<style scoped>
.bloc-modale {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
}

.overlay {
  background: rgba(0, 0, 0, 0.5);
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
}

.modale {
  background: #f1f1f1;
  color: black;
  padding: 30px;
  position: fixed;
  top: 30%;
}

.btn-modale {
  position: absolute;
  top: 10px;
  right: 10px;
  background-color: #790e3c;
  border-radius: 50%;
}
</style>
