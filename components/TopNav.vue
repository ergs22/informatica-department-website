<template>
  <div class="top-nav">
    <div class="container-logo">
      <NuxtLink to="/">
        <img
          src="../assets/images/Logo.svg"
          alt="departamento-informatica-logo"
        />
      </NuxtLink>
    </div>
    <div class="container-options">
      <div class="top-options">
        <nuxt-link to="/">
          <img src="../assets/icons/mdi_world.svg" alt="" />
          Idiomas</nuxt-link
        >
        <nuxt-link to="/">
          <img
            src="../assets/icons/mdi_contact.svg"
            alt=""
          />Contacto</nuxt-link
        >
      </div>
      <div class="bottom-options">
        <nuxt-link to="/">
          <img src="../assets/icons/vaadin_academy-cap.svg" alt="" /> Ofertas
          Academicas</nuxt-link
        >
        <nuxt-link to="/">
          <img
            src="../assets/icons/pepicons-pop_persons.svg"
            alt=""
          />Nosotros</nuxt-link
        >
        <nuxt-link to="/">
          <img
            src="../assets/icons/mdi_teacher.svg"
            alt=""
          />Profesores</nuxt-link
        >
        <nuxt-link to="/">
          <img src="../assets/icons/material-symbols_news.svg" alt="" />Noticias
          y eventos</nuxt-link
        >
      </div>
    </div>
  </div>
</template>

<style scoped>
.top-nav {
  padding: 0 2rem;
  display: flex;
  min-height: 117px;
  align-items: center;
  justify-content: space-between;
  background-color: #0d47a1;
  color: white;
  font-family: Poppins;
  font-size: 17.368px;
  font-style: normal;
  font-weight: 700;
  line-height: 20.988px;
}

.container-options {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.top-options,
.bottom-options {
  display: flex;
}

.container-options a {
  padding: 10px;
  display: flex;
  align-items: center;
}

.container-options a img {
  margin-right: 0.5rem;
}
.container-options a:hover {
  color: rgba(255, 255, 255, 0.596);
}
</style>
