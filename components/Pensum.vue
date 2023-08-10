<template>
  <section class="pensum">
    <h1>Pensum de estudios</h1>

    <div class="pensum-container" :style="{ backgroundImage: `url(${PM})` }">
      <div class="blur"></div>
      <button class="button">Descargar Pensum de estudio completo</button>
    </div>
  </section>
</template>

<script setup lang="js">
import PM from "../assets/images/pensum.svg";
</script>

<style scoped>
.pensum {
  text-align: center;
  padding-top: 4rem;
  padding-bottom: 3rem;
}
.pensum-container {
  position: relative;
  margin-top: 2rem;
  width: 100vw;
  min-height: 708px;
  background-size: cover;
  background-repeat: no-repeat;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}

.blur {
  position: absolute;
  width: 100%;
  height: 100%;

  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.26) 0%,
    rgba(255, 255, 255, 0.07) 100%
  );
  backdrop-filter: blur(5px);
  z-index: 1;
}
.button {
  min-width: 469px;
  height: 63px;
  padding: 9px 21.75px 9.063px 16.313px;
  gap: 7.25px;
  position: relative;
  z-index: 2;
  color: #fff;
  font-size: 19.416px;
  font-style: normal;
  font-weight: 700;
  line-height: 19.416px;
  border-radius: 5px;
  background: #1565c0;
  box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  overflow: hidden;
  transition: background-position 0.3s ease;
}

.button::before {
  content: "";
  position: absolute;
  left: -100%;
  top: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    to right,
    rgba(255, 255, 255, 0.363),
    transparent
  );
  transition: left 1s ease;
}

.button:hover::before {
  left: 100%;
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

p {
  color: #757575;
  font-size: 18.13px;
  font-style: normal;
  font-weight: 500;
  line-height: 28px;
}
</style>
