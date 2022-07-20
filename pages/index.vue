<template>
  <div class="container">
    <div class="containerOne">
      <h1>Salud mental para todos</h1>
    </div>
    <div class="containerTwo">
      <div>
        <img
          src="~/assets/img/index_img/dark-logo.png"
          alt="Crearte Consciencia - logo oscuro"
        />
      </div>
      <div class="textContainer">
        <h1>¿Qué es Crearte Consciencia?</h1>
        <p>
          Somos un equipo de psicólogos dedicado a la prestación de servicios de
          salud mental para personas e instituciones. Trabajamos por el
          mejoramiento de la calidad de vida de las personas desde la psicología
          clínica, enfatizando nuestros esfuerzos en el aumento de la
          accesibilidad a salud mental para todos los colombianos.
        </p>
      </div>
    </div>
    <div class="containerThree">
      <div class="textContainer">
        <h1>Integralidad</h1>
        <p>
          Somos un equipo de psicología integral. Esto significa que nuestra
          perspectiva en torno al ser humano y su salud mental se nutre de
          diferentes corrientes psicológicas, lo que nos permite dar una
          atención especializada, acorde a las necesidades de cada consultante o
          comunidad.
        </p>
      </div>
      <div>
        <img
          src="~/assets/img/index_img/team.png"
          alt="Grupo trabajando en equipo"
        />
      </div>
    </div>
    <div class="containerFour">
      <div>
        <img
          src="~/assets/img/index_img/great.png"
          alt="Dos personas chocando las manos"
        />
      </div>
      <div>
        <h1>Profesionales</h1>
        <p>
          Nuestro equipo de trabajo está conformado por psicólogos profesionales
          de los más altos estándares éticos. En Crearte Consciencia siempre
          estás en buenas manos.<br />

          Conoce a nuestro equipo <nuxt-link to="/nosotros">aquí</nuxt-link>.
        </p>
      </div>
    </div>
    <div class="containerFive">
      <div>
        <h1>Salud mental para todos</h1>
        <p>
          Democratizamos el acceso a la salud mental. Por esta razón, evaluamos
          si tus condiciones socioeconómicas son una dificultad para tu proceso,
          ofreciendo descuentos personalizados si es necesario. También
          implementamos proyectos sociales que mejoran la cobertura en salud
          mental.<br />
          ¡Contáctanos! Tu salud mental no debe ser un lujo.
        </p>
      </div>
      <div><img src="~/assets/img/index_img/hug.png" alt="" /></div>
    </div>
    <section class="gridContainer">
      <div>
        <i class="fa-solid fa-dollar-sign fa-3x" style="color: #85bc27"></i>
        <h1>Accesibilidad</h1>
        <p>
          La salud mental es un derecho de todos, sin importar las condiciones
          socioeconómicas particulares. Brindamos precios justos y asequibles
          para toda la población.
        </p>
      </div>
      <div>
        <i
          class="fa-solid fa-hand-holding-hand fa-3x"
          style="color: #f9b0be"
        ></i>
        <h1>Cobertura incomparable</h1>
        <p>
          No importa cuánto dure tu proceso, siempre estaremos a tu lado. Accede
          a todos los beneficios porque te cuidamos de inicio a fin.
        </p>
      </div>
      <div>
        <i
          class="fa-solid fa-face-smile-beam fa-3x"
          style="color: rgb(157, 225, 239)"
        ></i>
        <h1>Salud para todos</h1>
        <p>
          Proporcionamos servicios de salud mental para personas naturales y
          organizaciones. La salud mental debe ser la nueva normalidad.
        </p>
      </div>
      <div>
        <i class="fa-solid fa-calendar-check fa-3x" style="color: #ffbc63"></i>
        <h1>Responsabilidad social</h1>
        <p>
          Llegamos a las poblaciones más vulnerables planificando e
          implementando proyectos sociales enfocados en la promoción de la salud
          mental.
        </p>
      </div>
      <div>
        <i
          class="fa-solid fa-person-circle-check fa-3x"
          style="color: #60929b"
        ></i>
        <h1>Nos preocupamos por ti</h1>
        <p>
          Proporcionamos una sesión gratuita de valoración tras seis meses de
          finalizado tu proceso. Deseamos conocer tu evolución.
        </p>
      </div>
      <div>
        <i class="fa-solid fa-house-laptop fa-3x" style="color: #b27ce7"></i>
        <h1>Comodidad</h1>
        <p>
          Desde la comodidad de tu hogar o en el consultorio. En tu horario
          preferido. No hay excusas para darle un espacio a tu salud.
        </p>
      </div>
    </section>
  </div>
</template>

<style lang="scss">
.textContainer {
  @include customText;
}

.container {
  width: 100%;
  .containerOne {
    @include globalHeader(
      $customImage: url("~/assets/img/index_img/main-background.jpg"),
      $backgroundColor: rgba(153, 224, 244, 0.664)
    );
  }

  .containerTwo {
    @include bodyContentMain(
      $textColor: $darkColor,
      $backgroundColor: white,
      $height: 400px,
      $imgWidth: 200px
    );
  }

  .containerThree {
    @include bodyContentMain(
      $textColor: $clearColor,
      $backgroundColor: $mainColor,
      $height: 300,
      $imgWidth: 700px
    );
  }

  .containerFour {
    @include bodyContentMain(
      $textColor: $clearColor,
      $backgroundColor: $secundaryColor,
      $height: auto,
      $imgWidth: 1000px
    );
    background: linear-gradient(
      -177deg,
      $mainColor 0% 20%,
      $secundaryColor 20%
    );
    p {
      padding-left: 100px;
      padding-right: 100px;
    }
    a {
      color: $darkColor;
    }
    a:hover {
      color: rgb(86, 172, 243);
    }
  }

  .containerFive {
    @include bodyContentMain(
      $textColor: $clearColor,
      $backgroundColor: $secundaryColor,
      $height: auto,
      $imgWidth: 1200px
    );
    background: linear-gradient(
      -177deg,
      $secundaryColor 0% 20%,
      $mainColor 20%
    );
    p {
      padding-left: 100px;
      padding-right: 100px;
    }
  }
}

.gridContainer {
  @include featuresGrid();
  background: white;
  width: 100%;
  justify-content: center;
  align-content: center;
  padding: 70px 200px 70px 200px;
  div {
    @include featuresGridElement;
  }
}
</style>

<script>
import Vue from "vue";

export default Vue.extend({
  name: "IndexPage",
});
</script>