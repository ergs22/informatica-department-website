<template>
  <div class="card">
    <div><img :src="img" :alt="name" /></div>
    <h1>{{ name }}</h1>
    <p>{{ parraf }}</p>
  </div>
</template>

<script lang="js" setup>

const props = defineProps({
    name:String,
    parraf: String,
    img:String,
})
</script>

<style scoped>
.card {
  color: #263238;
  width: 337px;
  height: 305px;
  flex-shrink: 0;
  border-radius: 5px;
  background: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 0 1rem;
  transition: width 0.3s ease, height 0.3s ease, background-color 0.3s ease;
}

.card:hover {
  width: 350px;
  height: 340px;
  background: #e9e9e9;
  cursor: pointer;
}

.card div {
  margin-bottom: 1rem;
}

h1 {
  font-size: 18.625px;
  font-style: normal;
  font-weight: 800;
  line-height: 20px;
  margin-bottom: 1rem;
}

p {
  color: #757575;
  font-family: Roboto;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 20px;
}
</style>
