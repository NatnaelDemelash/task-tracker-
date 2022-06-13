<template>
  <button :style="{ background: color }" class="btn">{{ title }}</button>
</template>

<script>
export default {
  props: ["title", "color"],
};
</script>

<style lang="scss" scoped></style>
