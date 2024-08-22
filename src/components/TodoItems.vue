<script setup>
import TodoItem from "./TodoItem.vue";
</script>

<template>
  <!-- Todo items -->
  <div class="space-y-2">
    <TodoItem v-for="todo in $store.state.todos" :key="todo.id" :todo="todo" />
  </div>
  <!--/ Todo items -->
</template>
