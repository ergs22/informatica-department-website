<template>
  <div class="footer">
    <div class="main-container">
      <div class="container-option">
        <h1>Académicos</h1>
        <nuxt-link to="/">Programa de Pregrado</nuxt-link>
        <nuxt-link to="/">Oportunidades</nuxt-link>
        <nuxt-link to="/"> Recursos para estudiantes actuales </nuxt-link>
        <nuxt-link to="/"> Objetivos del programa y acreditación </nuxt-link>
      </div>

      <div class="container-option">
        <h1>Personal</h1>
        <nuxt-link to="/">Liderazgo</nuxt-link>
        <nuxt-link to="/">Profesores</nuxt-link>
      </div>

      <div class="container-option">
        <h1>Noticias y eventos</h1>
        <nuxt-link to="/">Noticias</nuxt-link>
        <nuxt-link to="/">Eventos</nuxt-link>
      </div>

      <div class="container-option">
        <h1>Acerca de nosotros</h1>
        <nuxt-link to="/">Hitoria Departamental</nuxt-link>
        <nuxt-link to="/">Organizacion Departamental</nuxt-link>
      </div>
    </div>
    <div class="secundary-container">
      <div class="container-left">
        <nuxt-link to="/">Accesibilidad</nuxt-link>
        <nuxt-link to="/">Disclaimer</nuxt-link>
        <nuxt-link to="/">Politicas de privacidad</nuxt-link>
      </div>

      <div class="container-logo">
        <img
          src="../assets//images/logo-footer.svg"
          alt="logo-departamento-informatica"
        />
      </div>

      <div class="container-right">
        <div class="social-medias">
          <nuxt-link to="/"> Facebook</nuxt-link>
          <nuxt-link to="/">Twitter</nuxt-link>
          <nuxt-link to="/">Instagram</nuxt-link>
          <nuxt-link to="/">Youtube</nuxt-link>
        </div>
        <div class="rights">
          <p>© 2023 UDO, todos lo derechos reservados</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.footer {
  background-color: #ffc600;
  color: black;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  font-style: normal;
  font-weight: 500;
  line-height: 18.126px;
}
.main-container {
  display: flex;
  justify-content: space-between;
  width: 90%;
  margin-bottom: 2rem;
}
.container-option {
  margin: 0 1rem;
  width: 20%;
}

.container-option h1 {
  font-style: normal;
  font-weight: 700;
  line-height: 20.988px;
}
.container-option a {
  display: block;
  margin: 1rem 0;
}

.secundary-container {
  display: flex;
  justify-content: space-between;
  width: 90%;
  align-items: flex-end;
}
.container-right .social-medias a {
  margin-left: 1rem;
}
.container-left a {
  margin-left: 1rem;
}
</style>
