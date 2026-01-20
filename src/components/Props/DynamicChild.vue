<template>
    <p v-for="skill in skills">{{ skill }}</p>
    <p v-for="user in users">{{ user }}</p>
</template>

<script>
    export default {
        props: {
            skills: Array,
            users: Array
        }
    }
</script>