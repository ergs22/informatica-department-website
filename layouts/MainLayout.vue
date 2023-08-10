<template>
  <TopNav />
  <div
    :class="route.fullPath === '/' ? 'w-full' : ''"
    class="mx-auto w-full px-0 body"
  >
    <slot />
  </div>
  <Footer />
</template>

<script setup>
const route = useRoute();
</script>

<style scoped>
.body {
  font-family: Poppins;
  background-color: #f5f5f5;
  overflow-x: hidden;
}
</style>
