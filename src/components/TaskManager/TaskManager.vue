<template>
  <div class="w-3/12 border-r">
    <h2 class="text-base uppercase text-center font-bold py-6 border-b">
      task manager
    </h2>
    <User />
    <!-- Projects component -->
    <div class="px-14 py-6 border-b">
      <h4 class="text-sm text-black font-bold uppercase">projects</h4>
      <ul class="flex items-center my-3">
        <i class="icon-size fa fa-circle-o text-purple-800"></i>
        <span class="text-sm ml-2">Marketing</span>
      </ul>
      <ul class="flex items-center my-3">
        <i class="icon-size fa fa-circle-o text-blue-800"></i>
        <span class="text-sm ml-2">Marketing</span>
      </ul>
      <ul class="flex items-center my-3">
        <i class="icon-size fa fa-circle-o text-yellow-600"></i>
        <span class="text-sm ml-2">Marketing</span>
      </ul>
      <ul class="flex items-center my-3">
        <i class="icon-size fa fa-circle-o text-red-800"></i>
        <span class="text-sm ml-2">Marketing</span>
      </ul>
    </div>
    <!--  End Project  -->
    <div class="px-14 py-6">
      <h4 class="text-sm text-black font-bold uppercase">TEAM</h4>
      <div class="flex overflow-x-auto my-3 items-center">
        <img
          src="https://i.pravatar.cc/30"
          class="rounded-full shadow-lg object-center mr-2 object-contain flex"
          alt=""
        />
        <img
          src="https://i.pravatar.cc/30"
          class="rounded-full shadow-lg object-center mr-2 object-contain flex"
          alt=""
        />
        <img
          src="https://i.pravatar.cc/30"
          class="rounded-full shadow-lg object-center mr-2 object-contain flex"
          alt=""
        />
        <img
          src="https://i.pravatar.cc/30"
          class="rounded-full shadow-lg object-center mr-2 object-contain flex"
          alt=""
        />
        <img
          src="https://i.pravatar.cc/30"
          class="rounded-full shadow-lg object-center mr-2 object-contain flex"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script>
import User from "./UserInfo/User";
export default {
  components: {
    User,
  },
};
</script>

<style scoped>
.icon-size {
  font-size: 10px;
  line-height: 10px;
}
</style>
