<template>
  <div id="app">
    <TodoList />
  </div>
</template>

<script>
import TodoList from "./components/TodoList";

export default {
  name: 'App',
  components: {
    TodoList
  }
}
</script>
