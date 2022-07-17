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
@include globalHeader($customImage: url("~/assets/img/index_img/main-background.jpg"), 
$backgroundColor: rgba(153, 224, 244, 0.664));
}
</style>

<script>
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage",
});
</script>