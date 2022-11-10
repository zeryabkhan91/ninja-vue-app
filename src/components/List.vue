<template>
  <div class="list-items">
    <a v-for="item in list_items" :key="item.title" :href="item.link" class="item">
      <div class="item-child">
        <span class="icon">
          <i class="fab fa-youtube"></i>
        </span>
        <div class="title">
          {{ item.title }}
        </div>
        <div>
        </div>
      </div>
    </a>
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
.list-items {
  margin-top: 20px;
}
.item {
  padding: 20px;
  border-radius: var(--border-radius,1rem);
  margin-block: 20px;
  text-decoration: none;
  color: black;
  display: block;
  border: 2px solid var(--items-border-color,#fff);
  background-color: var(--items-background-color,#fff);
  -webkit-backdrop-filter: var(--block-background-filter,none);
  backdrop-filter: var(--block-background-filter,none);
  -webkit-transition: background-color .3s ease,border-color .3s ease;
  transition: background-color .3s ease,border-color .3s ease;
}
.item:hover {
  background-color: var(--items-hover-background-color,#fff);
  color: var(--items-hover-text-color,inherit);
  cursor: pointer;
  border-color: var(--items-hover-border-color,transparent);
}

.item-child {
  display: flex;
  justify-content: space-between;
}
</style>
