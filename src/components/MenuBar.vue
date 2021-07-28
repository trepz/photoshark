<template>
  <div class="menu-bar">
    <div class="menu-item">File</div>
    <div class="menu-item">Edit</div>
  </div>
</template>

<script lang="ts">
import { ref, defineComponent } from 'vue'

export default defineComponent({
  name: 'menu-bar',
  setup: () => {}
})
</script>

<style scoped>
.menu-bar {
  background: var(--panel);
  padding: 4px;
  display: flex;
}
.menu-item {
  padding: 4px 12px;
  border-radius: 4px;
  cursor: default;
}
.menu-item:hover {
  background: var(--dark);
}
</style>