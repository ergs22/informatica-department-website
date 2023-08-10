<template>
  <section class="research">
    <h1>Áreas de investigación</h1>
    <p>
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Molestias,
      necessitatibus!
    </p>

    <div class="card-container">
      <Card
        v-for="element in data"
        :name="element.name"
        :parraf="element.parraf"
        :img="element.img"
        :key="element.id"
      />
    </div>
  </section>
</template>

<script setup lang="js">
import Card from "./Card.vue";
import IA from "../assets/images/ia-img.svg"
import GA from "../assets/images/gerencia-img.svg"
import IO from "../assets/images/inv-operaciones-img.svg"
import MA from "../assets/images/matematica-img.svg"
import RS from "../assets/images/redes-img.svg"
import SI from "../assets/images/sis-informacion-img.svg"

const data= [{
    name:"Gerencia",
    parraf:"lorem",
    img:GA,
    id:"1",
},
{
    name:"Investigacion de operaciones",
    parraf:"lorem",
    img:IO,
    id:"2",
},
{
    name:"Sistemas de información",
    parraf:"lorem",
    img:SI,
    id:"3",
},
{
    name:"Redes",
    parraf:"lorem",
    img:RS,
    id:"4",
}
,{
    name:"Matematica",
    parraf:"lorem",
    img:MA,
    id:"5",
},
{
    name:"Inteligencia Artificial",
    parraf:"lorem",
    img:IA,
    id:"6",
}]
</script>

<style scoped>
.research {
  text-align: center;
  padding-top: 4rem;
  padding-bottom: 3rem;
}

h1 {
  color: #1565c0;
  text-align: center;
  font-size: 45px;
  font-style: normal;
  font-weight: 800;
  line-height: 53.006px;
}

p {
  color: #757575;
  font-size: 18.13px;
  font-style: normal;
  font-weight: 500;
  line-height: 28px;
}
.card-container {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  margin: 2rem 0.5rem 0 0.5rem;
}

.card-container div {
  margin: 1rem;
}
</style>
