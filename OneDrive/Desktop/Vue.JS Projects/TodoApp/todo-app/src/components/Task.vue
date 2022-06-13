<template>
  <div :class="[task.reminder ? 'reminder' : '', 'task']">
    <h3>
      {{ task.text }}
      <i @click="onDelete(task.id)" class="fas fa-times"></i>
    </h3>
    <p>{{ task.date }}</p>
  </div>
</template>

<script>
export default {
  props: {
    task: Object,
  },
  methods: {
    onDelete(id) {
      this.$emit("delete-task", id);
    },
  },
};
</script>

<style lang="scss" scoped></style>
