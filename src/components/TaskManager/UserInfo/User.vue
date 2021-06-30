<template>
  <div class="py-6 border-b">
    <div class="text-center">
      <div class="flex justify-center">
        <img
          src="https://i.pravatar.cc/50"
          class="rounded-full shadow-lg object-center object-contain flex"
          alt=""
        />
      </div>
    </div>
    <span class="block font-bold text-black text-center mb-2">Anonymous</span>
    <span class="block font-semibold text-xs text-center"
      >anonymous@random.com</span
    >
    <div class="flex items-center justify-center py-2">
      <span class="block text-gray">
        <IconsLayout :type="'cog'" />
      </span>
      <span class="block text-gray mx-2">
        <IconsLayout :type="'message'" :notify="2" />
      </span>
      <span class="block text-gray">
        <IconsLayout :type="'bell'" :notify="3" />
      </span>
    </div>
    <!-- Task Component -->
    <div class="my-2 flex flex-col justify-center items-center">
      <div class="w-full">
        <p style="position:relative;left:220px">3/4</p>
      </div>
      <progress id="file" value="32" max="100"> 32% </progress>
    </div>
    <div class="flex justify-center">
      <div class="block mr-6">
        <span class="font-bold block text-sm text-center text-black">
          12
        </span>
        <p class="text-xs text-center">
          <span class="block font-bold">Completed</span>
          <span class="block">tasks</span>
        </p>
      </div>
      <div class="block mr-6">
        <span class="font-bold block text-sm text-center text-black">
          12
        </span>
        <p class="text-xs text-center">
          <span class="block font-bold">To do</span>
          <span class="block">tasks</span>
        </p>
      </div>
      <div class="block">
        <span class="font-bold block text-sm text-center text-black">
          12
        </span>
        <p class="text-xs text-center">
          <span class="block font-bold">All</span>
          <span class="block">completed</span>
        </p>
      </div>
      <!-- <div class="flex">
        <span class="font-bold block text-sm text-black">
          22
        </span>
        <span class="text-xs text-center">Todo<br />tasks</span>
      </div>
      <div class="flex">
        <span class="font-bold block text-sm text-black">
          243
        </span>
        <span class="text-xs text-center">All<br />completed</span>
      </div> -->
    </div>
  </div>
</template>

<script>
import IconsLayout from "./IconsLayout";
export default {
  components: {
    IconsLayout,
  },
};
</script>

<style scoped>
progress::-webkit-progress-bar {
  background-color: #e6edf8;
  border-radius: 7px;
  height: 8px;
}
progress::-webkit-progress-value {
  background-color: #547cff;
  border-radius: 7px;
}
</style>
