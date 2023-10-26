<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HeaderComponent from "@/components/HeaderComponent.vue";
</script>

<template>

  <div class="header-con">
    <HeaderComponent />
  </div>


  <RouterView />
</template>

<style scoped>

</style>
