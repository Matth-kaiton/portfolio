<script setup>
import ProfilePicture from '../atoms/ProfilePicture.vue';

    defineProps({
    content : {
        type: String,
        required: true,
    }
    })
</script>
<template>
    <section class="intro neon wrap">
        <p>{{ content }}</p>
        <ProfilePicture />
    </section>
</template>

<style scoped>
.intro {
  background-color: var(--p-c-background-secondary);
  display: flex;
  flex-direction: column;
  border: 2px solid rgb(56, 54, 54);
  border-radius: 15px;
  width: 60%;
}

.wrap{
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 1rem;
    padding: 1rem;
    align-items: center;
}


@media (min-width: 1024px) {

  .wrap{
    flex-direction: row-reverse;
  }
  

}
</style>