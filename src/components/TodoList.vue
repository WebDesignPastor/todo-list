<template>
  <div>
    <h1>My Todo List</h1>
    <ul>
      <li v-for="(todo, index) in todos" :key="index">
        {{ todo }}
      </li>
    </ul>
    <input type="text" v-model="newTodo" />
    <button @click="addTodo">Add Todo</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newTodo: "",
      todos: ["Learn Vue", "Practice Vue", "Master Vue"],
    };
  },
  methods: {
    addTodo() {
      this.todos.push(this.newTodo);
      this.newTodo = "";
    },
  },
};
</script>
