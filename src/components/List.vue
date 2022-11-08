<template>
  <div class="container">
    <div v-for="item in list_items" :key="item.title" class="item">
      {{ item.title }}
    </div>
  </div>
</template>

<script>
export default {
  name: "list-items",
  props: {
    list_items: {
      type: Array,
      default: () => [],
    },
  },
};
</script>

<style scoped>
.container {
  display: block;
  max-width: 640px;
}
.item {
  display: block;
}
</style>
