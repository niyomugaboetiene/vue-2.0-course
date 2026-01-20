<template>
    <DynamicChild :skills="skills" :users="users" />
</template>

<script>
    import DynamicChild from './DynamicChild.vue';
    export default {
        components: { DynamicChild },
        data() {
            return {
                skills: ["Vue", "React", "Javascript"],
                users: ["Anna", "Alice", "Emmy"]
            }
        }
    }
</script>