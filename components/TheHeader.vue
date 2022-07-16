<template>
  <div class="myNav">
    <nuxt-link to="/"
      ><img src="~/assets/img/icon.png" alt="Crearte Consciencia logo"></nuxt-link>
    <nuxt-link to="/" active-class="active">Inicio</nuxt-link>
    <div class="dropdown">
      <button class="dropdown-btn">
        Salud mental
        <i
          class="fa-solid fa-angle-down fa-xs"
          style="padding-left: 1px; color: aliceblue"
        ></i>
      </button>
      <div class="dropdown-content">
        <nuxt-link active-class="active" to="/personas">Personas</nuxt-link>
        <nuxt-link active-class="active" to="/organizaciones"
          >Organizaciones</nuxt-link
        >
      </div>
    </div>
    <nuxt-link active-class="active" to="/desarrollo-social"
      >Desarrollo social</nuxt-link
    >
    <nuxt-link active-class="active" to="/nosotros">Nosotros</nuxt-link>
    <div class="btnArea">
      <nuxt-link to="/contacto">
        <call-to-action></call-to-action>
      </nuxt-link>
    </div>
  </div>
</template>

<style lang="scss">
img {
  padding-right: 30px;
  width: 200px;
}
.myNav {
  padding: 10px;
  float: center;
  width: 100%;
  background-color: $mainColor;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  overflow: hidden;

  a {
    float: left;
    text-align: center;
    padding-right: 20px;
    padding-right: 20px;
    font-family: $globalFont;
    font-size: 18px;
    font-weight: bold;
    color: $clearColor;
    text-decoration: none;
    display: block;
  }
}

a:hover {
  color: $secundaryColor;
}
a.nuxt-link-exact-active {
  color: $secundaryColor;
  font-weight: bold;
}

.dropdown {
  align-items: center;
  justify-content: center;
  align-content: center;
  padding-right: 14px;
  .dropdown-btn {
    color: $clearColor;
    font-family: $globalFont;
    font-size: 18px;
    font-weight: bold;
  }
  .dropdown-btn:hover {
    color: $secundaryColor;
  }
}

.dropdown:hover {
  .dropdown-content {
    display: block;
    color: $secundaryColor;
  }
}
.dropdown-content {
  padding: 10px;
  display: none;
  position: absolute;
  z-index: 1;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.385);
  background-color: rgb(73, 75, 77);
  border-radius: 10px;
  a {
    float: none;
    text-align: left;
    padding: 5px;
  }
}

.btnArea {
  padding-left: 30px;
}
</style>