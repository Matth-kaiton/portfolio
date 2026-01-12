<script setup lang="ts">
import IconAncorBar from '../atoms/IconAncorBar.vue';
import '@/assets/base.css';
</script>

<template>
    <article class="spliter">
        <div class="spliterDecoration"></div>
        <IconAncorBar/>
        <div class="spliterDecoration"></div>
    </article>
</template>

<style scoped>
  .spliter {
    display: flex;
    flex: 1;
    width: 100%;
    align-items: center;
    justify-content: space-evenly;
    padding: 1rem ;
  }
    
  .spliterDecoration {
    background-color: var(--p-c-primary) ;
    height: 10px;
    flex: 1;
    border-radius: 10px;
  }
</style>