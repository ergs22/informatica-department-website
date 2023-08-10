<template>
  <div class="ticketSupport-container">
    <p>{{ parraf }}</p>
    <i
      class="ticketSupport-icon"
      :style="{ backgroundImage: `url(${moreIcon})` }"
    ></i>
  </div>
</template>

<script setup lang="js">
const props = defineProps({
    parraf: String,
})

import moreIcon from "../assets/icons/more-icon.svg"
</script>

<style scoped>
.ticketSupport-container {
  display: flex;
  width: 722px;
  height: 102px;
  justify-content: space-evenly;
  align-items: center;
  flex-shrink: 0;
  border-radius: 5px;
  background: #90caf9;
  transition: background-color 0.3s ease; /* Agregamos la transición */
}
.ticketSupport-container:hover {
  background-color: #64b5f6;
  cursor: pointer;
}
p {
  color: #263238;
  font-size: 20.48px;
  font-style: normal;
  font-weight: 700;
  width: 80%;
  height: 75px;
  overflow: hidden;
  line-height: 30.72px; /* 150% */
  display: flex;
  align-items: center;
}

.ticketSupport-icon {
  width: 38px;
  height: 38px;
  cursor: pointer;
}
</style>
