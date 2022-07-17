<template>
  <div class="container">
    <div class="containerOne">
      <h1>Salud mental para todos</h1>
    </div>
    <div class="containerTwo">
      <div>
        <img src="~/assets/img/index_img/dark-logo.png" alt="Crearte Consciencia - logo oscuro">
      </div>
      <div class="textContainer">
        <h1>¿Qué es Crearte Consciencia?</h1>
      <p>Somos un equipo de psicólogos dedicado a la prestación de servicios de salud mental para personas e instituciones. 
        Trabajamos por el mejoramiento de la calidad de vida de las personas desde la psicología clínica, enfatizando nuestros 
        esfuerzos en el aumento de la accesibilidad a salud mental para todos los colombianos. </p></div>
    </div>
  </div>
</template>

<style lang="scss">

.container{
  width: 100%;
  .containerOne {
  @include globalHeader(
    $customImage: url("~/assets/img/index_img/main-background.jpg"),
    $backgroundColor: rgba(153, 224, 244, 0.664)
  );
}

.containerTwo {
  @include bodyContentMain($clearText: true, $backgroundColor: white, $height: 400px, $imgHeight: 200);

  .textContainer{
    @include customText;
  }
}
}

</style>

<script>
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage",
});
</script>