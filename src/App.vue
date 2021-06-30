<template>
  <TaskLayout />
</template>

<script>
import TaskLayout from "./components/TaskLayout.vue";

export default {
  name: "App",
  components: {
    TaskLayout,
  },
};
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
