<template>
  <div class="py-5 border-b pl-4 pr-12 flex justify-between">
    <div class="w-2/12">
      <CheckMark :solid="true" />
    </div>
    <div class="w-10/12">
      <h4 class="text-black font-bold mb-1">
        Write an article about design trends
      </h4>
      <span class="inline-flex items-center text-sm font-bold">
        <i class="fa fa-clock-o icon-size mr-2"></i>
        <span>12 March,2018</span>
      </span>
      <div class="my-8 text-sm font-semibold">
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iste
          perspiciatis, porro ducimus eligendi est explicabo vitae corrupti
          alias inventore dolore corporis atque ex neque! Nostrum asperiores
          expedita ad fugiat dicta!
        </p>
      </div>
      <hr />
      <div class="my-4">
        <div class="text-sm">
          <p>
            <span class="font-bold mr-2">Noah Oskva</span>
            <span class="mr-3">Added to marketing</span>
            <span>19 Jun,2018</span>
          </p>
          <p>
            <span class="font-bold mr-2">Noah Oskva</span>
            <span class="mr-3">Assigned to Natalie Smith</span>
            <span>19 Feb,2018</span>
          </p>
          <p>
            <span class="font-bold mr-2">Noah Oskva</span>
            <span class="mr-3">created task</span>
            <span>19 Feb,2018</span>
          </p>
        </div>
      </div>
      <hr />
      <div class="my-4 flex items-center">
        <div class="mr-2">
          <CheckMark :solid="true" :small="true" />
        </div>
        <p class="mr-2 text-primary font-semibold">
          Natalie completed this task
        </p>
        <p>24 Feb,2018</p>
      </div>
      <hr />
      <div class="my-8 flex items-center justify-between">
        <div class="flex items-center">
          <div class="mr-2">
            <IconsLayout :type="'file'" :rectangle="true" :large="true" />
          </div>
          <div>
            <p class="font-bold text-black">Article.docx</p>
            <p class="text-sm">added 25 Feb,2018</p>
          </div>
        </div>
        <div class="flex items-center">
          <span class="mr-4">
            <i class="fa fa-trash-o icon-size"></i>
          </span>
          <span>
            <i class="fa fa-cloud-download icon-size"></i>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CheckMark from "../TaskManager/CheckMark";
import IconsLayout from "../TaskManager/UserInfo/IconsLayout";
export default {
  components: {
    CheckMark,
    IconsLayout,
  },
};
</script>

<style></style>
