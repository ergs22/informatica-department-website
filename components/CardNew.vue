<template>
  <div class="cardNew">
    <div
      class="img-container"
      :style="{ backgroundImage: `url(${img})` }"
    ></div>
    <div class="info-container">
      <div class="text-container">
        <h1>{{ name }}</h1>
        <p>{{ parraf }}</p>
      </div>
      <div class="action-container">
        <img
          src="../assets//icons//material-symbols_arrow-circle-up-rounded.svg"
          alt="show-icon"
          class="show-icon"
        />
        <p>Leer mas sobre esta noticia</p>
      </div>
    </div>
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
.cardNew {
  color: #263238;
  width: 1115px;
  height: 325px;
  flex-shrink: 0;
  background: #fff;
  display: flex;
  justify-content: space-between;
  transition: width 0.3s ease, height 0.3s ease, background-color 0.3s ease;
}

.cardNew:hover {
  width: 1128px;
  height: 355px;
  background: #e9e9e9;
  cursor: pointer;
}

.cardNew div {
  margin-bottom: 1rem;
}

.img-container {
  width: 50%;
  height: 100%;
  flex-shrink: 0;
  background-size: cover;
  background-repeat: no-repeat;
}
.text-container {
  text-align: start;
  max-width: 90%;
  max-height: 90%;
}
.text-container h1 {
  color: #263238;
  font-family: Poppins;
  font-size: 35px;
  font-style: normal;
  font-weight: 700;
  line-height: 35px;
}

.text-container p {
  margin-top: 1.5rem;
  color: #263238;
  font-family: Roboto;
  font-size: 19.416px;
  font-style: normal;
  font-weight: 700;
  line-height: 22px;
}
/* 113.311% */
.info-container {
  height: 100%;
  width: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  padding-left: 4rem;
}

.action-container {
  display: flex;
  align-items: center;
}

.action-container p {
  padding-left: 1rem;
  color: #263238;
  font-family: Poppins;
  font-size: 19.416px;
  font-style: normal;
  font-weight: 700;
  line-height: 19.416px; /* 100% */
}
</style>
