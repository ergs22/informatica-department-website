<template>
  <div class="carousel">
    <div class="big" ref="big">
      <img src="../assets/images/carousel1.svg" alt="Imagen1" />
    </div>

    <ul class="dots">
      <li @click="next" class="dot left"></li>
      <li @click="next" class="dot"></li>
      <li @click="next" class="dot right"></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "CarouselComp",

  methods: {
    next(e) {
      const big = this.$refs.big;

      let position = e.target.className === "dot" ? 1 : 0;

      let operation = position * -50;

      big.style.transform = `translateX(${operation}%)`;
    },
  },
};
</script>

<style scoped>
.carousel {
  position: relative;
  width: 100%;
  height: 600px;
  transition: all 0.4s ease;
  overflow: hidden;
}
.options {
  position: absolute;
  display: flex;
  top: 4%;
  left: 80%;
  z-index: 1000;
  color: #fff;
  text-align: center;
  font-family: Poppins;
  font-style: normal;
  font-weight: 700;
  line-height: 15.848px;
}

.options a:hover {
  color: #ffffff8e;
}

.options a {
  padding: 1rem;
  display: flex;
  align-items: center;
}
.options a img {
  margin-right: 0.5rem;
}
.big {
  width: 100%;
  display: flex;
  flex-flow: row nowrap;
  align-items: center;
  transition: all 0.4s ease;
  border-radius: 1em;
  transition: all 0.5s ease;
  transform: translateX(0%);
}
.big img {
  width: 100%;
  transition: all 0.4s ease;
}

.dots {
  width: 5%;
  display: flex;
  justify-content: space-between;
  margin: 0 auto 0 auto;
  align-items: center;
  list-style: none;
  position: absolute;
  top: 90%;
  left: 0;
  right: 0;
}

.dot {
  background-color: rgba(220, 220, 220, 0.493);
  cursor: pointer;
  width: 1em;
  height: 1em;
  transition: all 0.4s ease;
  border-radius: 1em;
  background-size: cover;
}

.dot:hover {
  cursor: pointer;
  width: 2em;
  height: 2em;
  transition: all 0.4s ease;
  border-radius: 1em;
  background-size: cover;
  background-color: rgb(201, 199, 199);
}

.dot.left {
  transform: scaleX(-1);
}
</style>
