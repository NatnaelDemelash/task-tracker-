<template>
  <header>
    <h1>Task Tracker</h1>
    <Button title="Add Tasks" color="green" />
  </header>
  <Tasks :tasks="tasks" />
</template>

<script>
import Button from "./Button.vue";
export default {
  name: "Header",
  components: {
    Button,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
