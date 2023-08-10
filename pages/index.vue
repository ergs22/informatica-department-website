<template>
  <MainLayout>
    <!-- <div class="pt-[80px] w-[calc(100%-90px)] max-w-[690px]">
      <div v-for="post in $generalStore.posts" :key="post">
        <PostMain v-if="post" :post="post" />
      </div>
    </div> -->
    <Carousel />
    <Pensum />
    <Research />
    <News />
    <Support />
  </MainLayout>
</template>

<script setup>
import MainLayout from "~/layouts/MainLayout.vue";
import Carousel from "~/components/Carousel.vue";
import Research from "~/components/Research.vue";
import News from "~/components/News.vue";
import Pensum from "~/components/Pensum.vue";
import Support from "~/components/Support.vue";

// const { $generalStore } = useNuxtApp();
// onMounted(async () => {
//   try {
//     $generalStore.getAllUsersAndPosts();
//   } catch (error) {
//     console.log(error);
//   }
// });
</script>
