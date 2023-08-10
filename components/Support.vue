<template>
  <section class="support">
    <h1>Preguntas frecuentes</h1>
    <div class="support-container">
      <div
        class="support-image"
        :style="{ backgroundImage: `url(${supportImage})` }"
      ></div>
      <div class="ticket-container">
        <TicketSupport
          v-for="element in data"
          :parraf="element.parraf"
          :key="element.id"
        />
      </div>
    </div>
  </section>
</template>

<script setup lang="js">
import TicketSupport from './TicketSupport.vue';
import supportImage from "../assets/images/faq-img.svg"


const data= [{
    parraf:"¿Qué opciones de becas y ayudas financieras existen para los estudiantes?",
    id:"1",
},
{
    parraf:"¿Qué documentos debo presentar para formalizar la matrícula?",
    id:"2",
},
{
    parraf:"¿Cómo puedo contactar con el profesorado, el personal administrativo y los servicios de la universidad?",
    id:"3",
},
{
    parraf:"¿Cómo puedo contactar con el profesorado, el personal administrativo y los servicios de la universidad?",
    id:"4",
}
]
</script>

<style scoped>
.support {
  padding-top: 4rem;
  padding-bottom: 3rem;
}
.support-container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 2rem 0 0 0;
}

.ticket-container div {
  margin: 2rem 0;
}
.support-image {
  width: 460px;
  height: 500px;
  flex-shrink: 0;
  background-size: cover;
  background-repeat: no-repeat;
}
h1 {
  color: #2196f3;
  margin-left: 8rem;
  text-align: start;
  font-size: 45px;
  font-style: normal;
  font-weight: 800;
  line-height: 53.006px;
}
</style>
