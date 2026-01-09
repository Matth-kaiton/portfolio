<script setup>
import ProfilePicture from '../atoms/ProfilePicture.vue';

    defineProps({
    title: {
        type: String,
        required: true,
    },
    content : {
        type: String,
        required: true,
    }
    })
</script>
<template>
    <section class="intro neon">
        <div class="test">
            <p>{{ content }}</p>
            <ProfilePicture />
        </div>
    </section>
</template>

<style scoped>
.intro {
  background-color: var(--p-c-background-secondary);
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 2px solid;
  border-color: var(--p-c-text-secondary);
  border-radius: 15px;
}

.test{
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 1rem;
    padding: 1rem;
    align-items: center;
}


@media (min-width: 1024px) {

  .test{
    flex-direction: row-reverse;
  }
  

}
</style>