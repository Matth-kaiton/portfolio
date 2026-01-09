<script setup>
  import ancorIcon from '@/assets/icons/ancorIcon.svg'
  import '@/assets/base.css';
</script>

<template>
  <img class="ancorIcon" :src="ancorIcon">
</template>

<style scoped>
.ancorIcon{
  width: 80px;
  height: 80px;
  rotate: 30deg;
  position: relative;
  top: -10px;
}
</style>
