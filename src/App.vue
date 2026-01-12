<script setup>
import './assets/main.css'
import Intro from './components/molecules/Intro.vue';
import Spliter from './components/molecules/Spliter.vue';

var text = "lorem ipsum"

</script>

<template>
  <div class="wrapper">
    <header>
      <h1>Portofilio Matthias DUMAS</h1>
      <Intro  :content=text />
    </header>
    <main>
      <Spliter/>
      <h2>mettre carouselle projet ou affichage grille ici</h2>
      <Spliter/>
      <h2>Mettre les compétence</h2>
      <Spliter/>
      <h2>info suplémentaire</h2>
      <Spliter/>
      <h2>Formulaire</h2>
    </main>
  </div>
</template>

<style scoped>

header {
  display: flex;
  width: 80%;
  flex-direction: column ;
  line-height: 1.5;
  padding: 0px;
  margin: auto;
}



@media (min-width: 1024px) {
  header {
    /* padding-right: calc(var(--section-gap) / 2);  a voir si on remet plus tard */
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
