<script setup>
  import './assets/main.css'
  import Card from './components/molecules/Card.vue';
  import Contact from './components/molecules/Contact.vue';
  import Intro from './components/molecules/Intro.vue';
  import Spliter from './components/molecules/Spliter.vue';
  import projects from "@/data/projects.json";
  import content from "@/data/content.json";
  import Training from './components/molecules/Training.vue';
  import Logo from './components/atoms/Logo.vue';
</script>

<template>
    <header>
    </header>
    <main>
      <h1>Portofilio Matthias DUMAS</h1>
      <Intro/>
      <Spliter/>
      <h2>Formation</h2>
      <section class="wrapTraining">
        <Training
          v-for="train in content.training"
          :title=train.name
          :location=train.location
          :level=train.level
          :years=train.years
          />
      </section>
      <h2>Compétence</h2>
      <section class="competence">
        <Logo
        v-for="logo in content.competence" 
        :source="logo.icon"
        :text="logo.text"
        />
      </section>
      <Spliter/>
      <h2>Projet</h2>
      <section class="projects">
        <Card 
        v-for="project in projects"
        :title=project.title
        :content=project.content
        :webp=project.webp
        :img=project.img
        :alt=project.alt
        :techno=project.techno
        :date=project.date
        :gitUrl=project.gitUrl
        />
      </section>
    </main>
</template>

<style scoped>

header {
  display: flex;
  width: 100%;
  flex-direction: column ;
  line-height: 1.5;
  padding: 0px;
  margin: auto;
}

main{
  flex:1;
  width: 100%;
  padding: 30px 0px;
  gap: 1rem;
}

.wrapTraining{
  display: flex;
  flex-direction: column;
  gap: 1rem;
}



@media (min-width: 1024px) {
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  .wrapTraining{
    flex-direction: row;
    gap: 1rem;
  }
}
</style>
