<script>
import TasksList from './components/TasksList.vue'

export default {
  name: 'App',
  components: {
    TasksList
  }
}
</script>


<template>
  <div id="app">
    <p>Tasks List</p>
    <TasksList/>
  </div>
</template>