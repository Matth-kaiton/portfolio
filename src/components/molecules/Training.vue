<script setup>

    defineProps({
        title : {String},
        location : {String},
        level : {String},
        years : {String}
    })
</script>

<template>
    <article class="training">
        <h3> {{ title }} </h3>
        <p> {{ location }} </p>
        <div>
            <p>{{ level }}</p>
            <p>{{ years }}</p>
        </div>
    </article>
</template>


<style scoped>
.training {
  max-width: 800px;
  padding: 2rem;

  background: var(--p-c-background-secondary);
  color: var(--p-c-text-primary);

  border-radius: 12px;
  border: 2px solid var(--p-c-background-secondary);

  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
  transition: transform 0.5s ease;
}

.training:hover {
    border: 2px solid var(--p-c-decoration);
    transform: scale(1.05);
}
</style>