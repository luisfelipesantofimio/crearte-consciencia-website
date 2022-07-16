<template>
  <div class="container">
    <div class="mainTitle">
      <h1>SÍGUENOS</h1>
    </div>
    <div class="iconsRow">
      <a target="_blank" href="https://www.instagram.com/crearteconsciencia.co/"
        ><i class="fa-brands fa-instagram fa-2x"></i
      ></a>
      <a target="_blank" href="https://www.facebook.com/CrearteConsciencia.co"
        ><i class="fa-brands fa-facebook fa-2x"></i
      ></a>
      <a
        target="_blank"
        href="https://www.linkedin.com/company/corporaci%C3%B3n-crearte-consciencia"
        ><i class="fa-brands fa-linkedin fa-2x"></i
      ></a>
    </div>
    <div class="footerContainer">
      <div class="footerElements">
        <div class="footerLogo">
          <img
            src="~/assets/img/footer-icon.png"
            alt="Crearte Consciencia - logo">
        </div>
        <div class="footerNav">
          <div class="navTitle"><p>Sitio</p></div>
          <div class="navElements">
            <nuxt-link to="/personas"><p>Personas</p></nuxt-link>
            <nuxt-link to="/organizaciones"><p>Organizaciones</p></nuxt-link>
            <nuxt-link to="/desarrollo-social"
              ><p>Desarrollo social</p></nuxt-link
            >
            <nuxt-link to="#"><p>Miembros</p></nuxt-link>
          </div>
        </div>
        <div class="footerNav">
          <div class="navTitle"><p>Acerca de</p></div>
          <div class="navElements">
            <nuxt-link to="/nosotros"><p>Nosotros</p></nuxt-link>
            <nuxt-link to="contacto"><p>Contáctanos</p></nuxt-link>
            <nuxt-link to="#"><p>Políticas de privacidad</p></nuxt-link>
            <nuxt-link to="#"><p>Política de cookies</p></nuxt-link>
            <nuxt-link to="#"><p>Términos de uso</p></nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.container {
  background-color: $footerBackground;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-bottom: 2rem;

  h1 {
    text-align: center;
  }

  p {
    font-family: $globalFont;
    font-size: 15px;
    padding-top: 5px;
  }

  a {
    font-family: $globalFont;
    font-size: 15px;
    padding-top: 5px;
  }
}

.mainTitle {
  h1 {
    color: #57838b;
    text-align: center;
    font-size: 25px;
    font-family: "Montserrat", sans-serif;
    font-weight: bold;
    justify-items: center;
    margin: 20px;
    margin-top: 50px;
  }
}

.iconsRow {
  i {
    align-items: center;
    flex-direction: row;
    color: aliceblue;
    padding: 10px;
    padding-left: 20px;
    padding-right: 20px;
    transition: 0.5s;
  }

  i:hover {
    color: #f9b0be;
  }
}

.footerContainer {
  padding: 20px;
  padding-top: 8rem;
  .footerElements {
    display: flex;
    flex-direction: row;
    .footerNav {
      flex-direction: column;
      padding-left: 50px;
      .navTitle p {
        color: #57838b;
        font-size: 20px;
        font-weight: bold;
      }
      .navElements a {
        color: aliceblue;
        transition: 0.5s;
      }

      .navElements a:hover {
        color: #f9b0be;
      }
    }
  }
  .footerLogo img {
    width: 250px;
  }
}
</style>

