<template>
  <menu-bar />
  <editor />
</template>

<script lang="ts">
import { defineComponent } from 'vue'

import Editor from './components/Editor.vue'
import MenuBar from './components/MenuBar.vue'
import ToolBar from './components/ToolBar.vue'
import ToolDetailsBar from './components/ToolDetailsBar.vue'

export default defineComponent({
  name: 'App',
  components: {
    Editor,
    MenuBar,
    ToolBar,
    ToolDetailsBar
  }
})
</script>

<style>
@import 'modern-css-reset';

#app {
  /* Colours */
  --dark: #252525;
  --panel: #303030;
  --text: #d5d5d5;

  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: var(--text);
  background: var(--dark);
  min-height: 100vh;
  min-width: 100vw;
}
</style>
