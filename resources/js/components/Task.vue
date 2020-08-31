<template>

        <tr>
            <td>{{task.title}}</td>
            <td>{{task.priority}}</td>
            <td>{{task.completed}}</td>
        </tr>

</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        },

        props: ['task']
    }
</script>

<style>

</style>
