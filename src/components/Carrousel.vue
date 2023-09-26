<template>
  <div class="carrousel">
    <div
      class="slide"
      :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
    >
      <img src="@/assets/Cahierdescharges-1.png" alt="Image 1" />
      <img src="@/assets/Cahierdescharges-2.png" alt="Image 2" />
      <img src="@/assets/Cahierdescharges-3.png" alt="Image 3" />
      <img src="@/assets/Cahierdescharges-4.png" alt="Image 4" />
      <img src="@/assets/Cahierdescharges-5.png" alt="Image 5" />
    </div>
    <div class="controls">
      <button @click="prevSlide" :disabled="currentIndex === 0">
        Précédent
      </button>
      <button @click="nextSlide" :disabled="currentIndex === images.length - 1">
        Suivant
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentIndex: 0,
      images: [
        "../assets/Cahierdescharges-1.png",
        "../assets/Cahierdescharges-2.png",
        "../assets/Cahierdescharges-3.png",
        "../assets/Cahierdescharges-4.png",
        "../assets/Cahierdescharges-5.png",
      ],
    };
  },
  methods: {
    prevSlide() {
      if (this.currentIndex > 0) {
        this.currentIndex--;
      }
    },
    nextSlide() {
      if (this.currentIndex < this.images.length - 1) {
        this.currentIndex++;
      }
    },
  },
};
</script>

<style scoped>
.carrousel {
  display: flex;
  overflow: hidden;
  position: relative;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  flex-direction: column;
}

.slide {
  display: flex;
  transition: transform 0.3s ease-in-out;
}

img {
  max-width: 100%;
  height: auto;
}

.controls {
  justify-content: space-between;
  margin-top: 1rem;
}

button {
  padding: 0.5rem 1rem;
  background-color: #007bff;
  color: #fff;
  border: none;
  cursor: pointer;
}

button:disabled {
  background-color: #ccc;
  cursor: not-allowed;
}
</style>
