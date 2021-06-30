<template>
  <div style="overflow-y:auto;height:69vh" class="border-r">
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
    <div
      id="tasks"
      class="bg-grayish p-5 flex items-center justify-between border-b"
    >
      <div class="flex">
        <div class="mr-2">
          <CheckMark :regular="true" />
        </div>
        <div class="text-xs">
          <p class="text-black font-bold">Create AdWords campaign</p>
          <p>22 Feb,2018</p>
        </div>
      </div>
      <img
        src="https://i.pravatar.cc/30"
        class="rounded-full shadow-lg object-center object-contain flex"
        alt=""
      />
    </div>
  </div>
</template>

<script>
import CheckMark from "../TaskManager/CheckMark";
export default {
  props: ["tasks"],
  components: {
    CheckMark,
  },
};
</script>

<style scoped>
/* width */
::-webkit-scrollbar {
  width: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #e6edf8;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #c4c7c7;
  border-radius: 10px;
}
</style>
