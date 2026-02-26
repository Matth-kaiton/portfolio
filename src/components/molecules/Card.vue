<script setup>
    defineProps({
        title : { String },
        content : { String },
        webp : { String },
        img : { String },
        alt : { String },
        techno : { Array },
        date : { String },
        gitUrl : { String }
    })
</script>

<template>
    <article class="card neon">
        <img class="card_img" :src="webp"/>
        <div class="wrap">
          <h3> {{ title }} </h3>
          <p> {{ content }} </p>
          <div class="card_tech">
            <span v-for="tech in techno" :key="tech">
             {{ tech }} 
            </span>
          </div>
          <p>{{ date }}</p>
          <a :href="gitUrl" target="_blank">GitHub</a>
        </div>
    </article>
</template>

<style scoped>

.card {
  background-color: var(--p-c-background-secondary);
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 2px solid rgb(56, 54, 54);
  border-radius: 15px;
  width: 95%;
  transition: transform 0.5s ease;
  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
  max-width: 300px;
}

.card:hover {
    border: 2px solid var(--p-c-decoration);
    transform: scale(1.05);
}

.card_img {
  width: 100%;
  height: auto;
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
  object-fit: cover;
}

.wrap{
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 1rem;
    padding: 1rem;
    align-items: center;
}

.card_tech{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.card_tech span{
  border: 1px solid var(--p-c-decoration);
  border-radius: 10px;
  padding: 0.2rem 0.5rem;
}

.wrap a:hover{
  background-color: unset;
}




@media (min-width: 1024px) {

  .test{
    flex-direction: row-reverse;
  }
  
  .card{
    width: 30%;
  }
  
}
</style>