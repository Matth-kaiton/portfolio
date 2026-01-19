<script setup>
import ProfilePicture from '../atoms/ProfilePicture.vue';
import content from "@/data/content.json";
</script>

<template>
    <section class="intro neon wrap">
        <div>
            <p  v-for="(text , i) in content.aboutMe" :key="i">{{ text }}</p>
        </div>
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
    flex-direction: column-reverse;
    justify-content: center;
    gap: 1rem;
    padding: 1rem;
    align-items: center;
    text-align: start;
    color: var(--p-c-text-secondary);
}


@media (min-width: 1024px) {

  .wrap{
    flex-direction: row-reverse;
  }
  

}
</style>