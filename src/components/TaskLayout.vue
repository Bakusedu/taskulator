<template>
  <div class="box shadow-lg flex text-gray-400">
    <TaskManager />
    <TaskBody />
  </div>
</template>

<script>
import TaskBody from "./TaskBody/TaskBody";
import TaskManager from "./TaskManager/TaskManager";
export default {
  components: {
    TaskBody,
    TaskManager,
  },
};
</script>
<style scoped>
.box {
  width: 1300px;
  margin: 0 auto;
}
</style>
