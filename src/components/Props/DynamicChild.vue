<template>
    <h1>{{ users.name }}</h1>
    <p v-for="skill in skills">{{ skill }}</p>
</template>

<script>
    export default {
        props: {
            skills: Array,
            users: Object
        }
    }
</script>