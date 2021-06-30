<template>
  <div class="w-9/12">
    <div class="p-4 flex items-center border-b justify-between">
      <div id="search" class="w-5/12" style="position:relative">
        <i
          class="fas fa-search icon-size absolute"
          style="top:13px;left:12px"
        ></i>
        <input
          type="text"
          name="search"
          class="rounded-lg pl-8 w-full outline-none py-2"
          id=""
        />
      </div>
      <div id="alltasks" class="w-7/12">
        <div class="flex pr-6 justify-between">
          <div class="flex items-center">
            <h4 class="text-black text-base font-semibold mr-2">All Tasks</h4>
            <span class="block">
              <i class="fas fa-chevron-down icon-size text-black"></i>
            </span>
          </div>
          <div class="flex items-center">
            <span class="block">
              <i class="fa fa-ellipsis-h icon-size"></i>
            </span>
          </div>
        </div>
      </div>
    </div>
    <div class="flex border-b">
      <div class="w-4/12">
        <div
          class="p-5 border-l-4 border-purple-600 flex items-center justify-between"
        >
          <div class="font-semibold">
            <span class="text-black text-sm uppercase">
              marketing
            </span>
          </div>
          <span class="block">
            <i class="fas fa-chevron-down icon-size text-black"></i>
          </span>
        </div>
      </div>
      <div class="w-8/12 border-l p-4 flex items-center justify-between">
        <div>
          <div class="flex items-center">
            <img
              src="https://i.pravatar.cc/30"
              class="rounded-full shadow-lg mr-2 object-center object-contain flex"
              alt=""
            />
            <span class="block text-black font-semibold text-sm"
              >Anonymous</span
            >
          </div>
        </div>
        <div>
          <IconsLayout class="mr-3" :type="'trash'" />
          <IconsLayout class="mr-3" :type="'user'" />
          <IconsLayout class="mr-3" :type="'tag'" />
          <IconsLayout class="mr-3" :type="'checkbox'" />
          <IconsLayout class="mr-3" :type="'paperclip'" />
        </div>
      </div>
    </div>
    <div class="flex">
      <div class="w-4/12">
        <Tasks />
        <div class="py-9 flex justify-center">
          <button class="bg-primary py-2 px-6 rounded-full text-white">
            Add task
          </button>
        </div>
      </div>
      <div class="w-8/12">
        <TaskView />
        <div class="flex border-l">
          <div class="w-8/12 border-r bg-grayish">
            <div class="p-5">
              <textarea
                name=""
                id=""
                class="w-full outline-none bg-grayish resize-none"
                placeholder="Write a comment"
                rows="3"
              ></textarea>
            </div>
          </div>
          <div class="w-4/12 flex bg-grayish">
            <div class="flex flex-col w-1/2 items-center justify-center">
              <span>
                <i class="icon-size fa fa-paperclip"></i>
              </span>
            </div>
            <div
              class="flex flex-col w-1/2 items-center bg-primary justify-center"
            >
              <span>
                <i class="icon-size fa fa-share text-white"></i>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import IconsLayout from "../TaskManager/UserInfo/IconsLayout";
import TaskView from "./TaskView";
import Tasks from "../TaskBody/Tasks";
// import CheckMark from "../TaskManager/CheckMark";
export default {
  components: {
    IconsLayout,
    TaskView,
    Tasks,
    // CheckMark,
  },
};
</script>

<style></style>
