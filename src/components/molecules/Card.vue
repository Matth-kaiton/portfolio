<script setup>
import ProfilePicture from '../atoms/ProfilePicture.vue';

    defineProps({
    title: {
        type: String,
        required: true,
    },
    content : {
        type: String,
        required: true,
    }
    })
</script>
<template>
    <div>
        <h1>{{ title }}</h1>
        <p>{{ content }}</p>
        <ProfilePicture />
    </div>
</template>