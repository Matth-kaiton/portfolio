<script setup>
import './assets/main.css'
import NavBtn from './components/atoms/NavBtn.vue';
import Card from './components/molecules/Card.vue';
import NavAncor from './components/molecules/NavAncor.vue';
</script>

<template>
  <div class="test">
    <header>
      <NavBtn/>
      <Card class="card" title="coucou" content="salut moi c'est matthias" />
    </header>
    <main>
      <NavAncor/>
    </main>
  </div>
</template>

<style scoped>
header {
  display: flex;
  flex-direction: column ;
  line-height: 1.5;
  outline: 2px solid red;
}

main {
  outline: 2px solid blue;
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
