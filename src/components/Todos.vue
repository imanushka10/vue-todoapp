<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <TodoItem v-bind:todo="todo" />
    </div>
  </div>
</template>



<script>
import TodoItem from "./TodoItem";
export default {
  name: "Todos",
  components: {
    TodoItem,
  },
  props: ["todos"], //Name of Components
};
</script>





<style scoped>
</style>