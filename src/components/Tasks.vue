<template>
    <div v-for="task in tasks" :key="task.id">
        <Task :task="task" />
    </div>
</template>

<script>
  import Task from './Task'

  export default {
    name: 'TaskList',
    props: {
      tasks: Array
    },
    components: {
      Task,
    },
  }
</script>