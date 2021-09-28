<template>
  <header>
    <h1>{{ text }}</h1>
    <Button
      @toggle-add-task="$emit('toggle-add-task')"
      :color="showAddTask ? 'red' : 'green'"
      :text="showAddTask ? 'Close' : 'Add Task'"
    />
  </header>
</template>
<script>
import Button from "./Button.vue";
export default {
  name: "Header",
  components: { Button },
  props: {
    text: String,
    showAddTask: Boolean
  }
};
</script>
<style scoped>
header {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
  color: blue;
}
</style>
