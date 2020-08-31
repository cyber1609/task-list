<template>
    <div class="app-component">
        <table class="table">
            <tr>
                <th>Task title</th>
                <th>Priority</th>
                <th>Completed</th>
            </tr>
            <task-component v-for="task in tasks" :key="task.id" :task="task"></task-component>

        </table>
    </div>
</template>

<script>
    import TaskComponent from './Task.vue'
    export default {
        mounted() {
            console.log('Component mounted.')
        },
        data() {
            return {

                tasks: [
                    {id: 1, title: 'Task 1', priority: 2, completed: false},
                    {id: 2, title: 'Task 2', priority: 9, completed: false},
                    {id: 3, title: 'Task 3', priority: 5, completed: true}
                ]

            }
        },
        components: {TaskComponent}
    }
</script>

<style>

</style>
