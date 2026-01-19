<script>

    defineProps({
        title : {String},
        location : {String},
        level : {String},
        years : {String}
    })
</script>

<template>
    <article>
        <h2> {{ title }} </h2>
        <p> {{ location }} </p>
        <div>
            <p>{{ level }}</p>
            <p>{{ years }}</p>
        </div>
    </article>
</template>
