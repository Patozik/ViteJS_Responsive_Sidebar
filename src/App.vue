<template>
  <div class="app">
    <Sidebar />

    <router-view />
  </div>
</template>

<script setup>
import Sidebar from './components/SideBar.vue'
</script>

<style lang="scss">

:root {
  --primary: #ff4000;
  --primary-alt: #ff6633;
  --grey: #696969;
  --dark: #262626;
  --dark-alt: #363636;
  --light: #b8b8b8;
  --sidebar-width: 300px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Open Sans', sans-serif;
}

body {
  background: var(--light);
}

button {
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  background: none;
}

.app {
  display: flex;

  main {
    flex: 1 1 0;
    padding: 2rem;

    @media (max-width: 768px) {
      padding-left: 6rem;
    }
  }
}

</style>
