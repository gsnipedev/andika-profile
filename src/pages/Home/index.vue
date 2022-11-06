<script lang="ts">
export default {
  data() {
    return {
      temp: "",
      todos: [] as string[],
    };
  },
  methods: {
    addTodo(e: Event, temp2: string) {
      e.preventDefault();
      if (!this.temp) return;

      this.todos.push(temp2);
      this.temp = "";
      return;
    },
  },
};
</script>

<template></template>

<style scoped></style>
