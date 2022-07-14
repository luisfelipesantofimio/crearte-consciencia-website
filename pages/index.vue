<template>
  <div class="container">
    <div class="containerOne">
      <h1>Salud mental para todos</h1>
    </div>
  </div>
</template>

<style>
.containerOne {
  display: flex;
  position: relative;
  height: 500px;
  width: 100%;
  background: url("~/assets/img/index_img/main-background.jpg"),#99e9ff;;
  background-size: cover;
  background-position: center;
  align-items: center;
  justify-content: center;
}

.containerOne::before{
  background-color: rgba(153, 191, 244, 0.595);
  content: '';
  display: block;
  height: 100%;
  position: absolute;
  width: 100%;
}

.containerOne h1 {
  color: aliceblue;
  text-align: center;
  vertical-align: middle;
  font-size: 50px;
  z-index: 1;
}
</style>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>