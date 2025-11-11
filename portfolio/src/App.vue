<script setup>
import HelloWorld from './components/HelloWorld.vue'
import ProfilePicture from './components/atoms/ProfilePicture.vue';
import TheWelcome from './components/TheWelcome.vue'
import NavBtn from './components/atoms/NavBtn.vue';
import PText from './components/atoms/PText.vue';
import TitleText from './components/atoms/TitleText.vue';
</script>

<template>
  <header>
    
    <NavBtn/>
    <div class="wrapper">
      <HelloWorld msg="You did it!" />
      <TitleText title="Menu" />
      <PText text="hello la team" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
