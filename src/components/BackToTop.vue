<template>
  <div class="back-to-top">
    <img
      src="../assets/Gototop.png"
      alt="back-to-top"
      id="logototop"
      class="btn btn-primary"
      @click="scrollToTop"
    />
  </div>
</template>

<script>
export default {
  methods: {
    scrollToTop() {
      window.scrollTo({ top: 0, left: 0 });
    },
  },
};
</script>

<style>
.back-to-top {
  position: fixed;
  bottom: 20px;
  right: 20px;
  z-index: 9999;
}

.logo {
  width: 20px;
  height: 20px;
}

#logototop {
  height: 50px;
}
</style>
