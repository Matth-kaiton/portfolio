<script setup>
defineProps({
  source: {
    type: String,
    required: true,
  },
  text: {
    type: String,
    required: true,
  },
})
</script>

<template>
    <img class="comp" :src=source :alt=text >
</template>



<style scoped>

.comp{
  width: 60px;
  transition: transform 0.5s ease;
}


.comp:hover{
  transform: scale(1.25)
}
</style>