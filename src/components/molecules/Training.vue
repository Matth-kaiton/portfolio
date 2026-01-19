<script setup>

    defineProps({
        title : {String},
        location : {String},
        level : {String},
        years : {String}
    })
</script>

<template>
    <article>
        <h3> {{ title }} </h3>
        <p> {{ location }} </p>
        <div>
            <p>{{ level }}</p>
            <p>{{ years }}</p>
        </div>
    </article>
</template>
