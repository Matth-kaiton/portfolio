<script setup lang="ts">
import IconAncorBar from '../atoms/IconAncorBar.vue';
import '@/assets/base.css';
</script>

<template>
    <nav class="ancor">
        <div class="ancorDecoration"></div>
        <IconAncorBar/>
        <div class="ancorDecoration"></div>
    </nav>
</template>

<style scoped>
  .ancor {
    display: flex;
    flex: 1;
    width: 100%;
  }
    
  .ancorDecoration {
    background-color: var(--p-c-decoration) ;
    width: 10px;
    height: 10px;
  }
</style>