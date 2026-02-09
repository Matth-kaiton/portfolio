<script setup>
    defineProps({
        title : { String,},
        content : { String, },
        webp : { String },
        img : { String },
        alter : { String }
    })
</script>

<template>
    <article class="card neon">
        <img :src="webp"/>
        <div class="wrap">
            <h3> {{ title }} </h3>
            <p> {{ content }} </p>
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
  width: 60%;
  transition: transform 0.5s ease;
  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

.card:hover {
    border: 2px solid var(--p-c-decoration);
    transform: scale(1.05);
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

  .test{
    flex-direction: row-reverse;
  }
  
  .card{
    width: 30%;
  }
  
}
</style>