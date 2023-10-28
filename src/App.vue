<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HeaderComponent from "@/components/HeaderComponent.vue";
import HomePage from "@/components/HomePage.vue";
import FooterComponent from "@/components/FooterComponent.vue";
</script>

<template>

  <div class="header-con">
    <HeaderComponent />
  </div>




  <RouterView />

  <div>
    <FooterComponent />
  </div>
</template>

<style scoped>

</style>
