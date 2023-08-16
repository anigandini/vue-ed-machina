<script setup lang="ts">
  import Header from './components/Header.vue'
</script>

<template>
  <Header></Header>
</template>

<style>
:root {
  --primary: rgba(68, 54, 253, 1);
  --secondary: rgba(115, 103, 240, 1);
  --bg: rgba(248, 248, 248, 1);
  --bg-light: rgba(255, 255, 255, 1);
  --gray-s: rgba(110, 107, 123, 1);
  --gray-m: rgba(238, 238, 238, 1);
  --green: rgba(40, 199, 111, 1);
  }
  #app {
    padding: 0 !important;
    margin: 0 !important;
    box-sizing: border-box;

  }
  body {
    margin: 0;
    max-width: 100%;
    overflow-x: hidden;
    font-family: 'Montserrat', sans-serif;
    line-height: 14.63px;
  }

</style>
