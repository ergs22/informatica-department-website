<template>
  <section class="research">
    <h1>Noticias</h1>
    <div class="card-container">
      <CardNew
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
import CardNew from "./CardNew.vue";
import newOne from "../assets/images/new-one.svg"
import newTwo from "../assets/images/new-two.svg"
import newThree from "../assets/images/new-three.svg"


const data= [{
    name:"Gala musical universitaria",
    parraf:"There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form",
    img:newOne,
    id:"1",
},
{
    name:"Inician las actividades academicas",
    parraf:"If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden in the.",
    img:newTwo,
    id:"2",
},
{
    name:"Nuevo Núcleo en Sucre",
    parraf:"There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form",
    img:newThree,
    id:"3",
},
]
</script>

<style scoped>
.research {
  text-align: center;
  padding-top: 4rem;
  padding-bottom: 3rem;
}

h1 {
  color: #1565c0;
  margin-left: 8rem;

  text-align: start;
  font-size: 45px;
  font-style: normal;
  font-weight: 800;
  line-height: 53.006px;
}

.card-container {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  margin: 2rem 0.5rem 0 0.5rem;
}

.card-container div {
  margin: 3rem;
}
</style>
