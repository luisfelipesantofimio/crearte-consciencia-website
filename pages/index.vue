<template>
  <div class="container">
    <div class="containerOne">
      <h1>Salud mental para todos</h1>
    </div>
    <div>
      <div></div>
      <div></div>
    </div>
  </div>
</template>

<style lang="scss">
/* TODO: Create global header for all pages with Sass */
.containerOne {
  display: flex;
  position: relative;
  height: 500px;
  width: 100%;
  background: url("~/assets/img/index_img/main-background.jpg"), #99e9ff;
  background-size: cover;
  background-position: center;
  align-items: center;
  justify-content: center;

  h1 {
    color: $clearColor;
    text-align: center;
    vertical-align: middle;
    font-family: $globalFont;
    font-size: 40px;
    font-weight: bold;
    z-index: 1;
  }
}

.containerOne::before {
  background-color: rgba(153, 224, 244, 0.664);
  content: "";
  display: block;
  height: 100%;
  position: absolute;
  width: 100%;
}
</style>

<script>
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage",
});
</script>