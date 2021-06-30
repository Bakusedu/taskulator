<template>
  <span style="position:relative">
    <i
      class="p-2 bg-grayish text-primary"
      :class="IconType + ' ' + borderRadius + ' ' + size"
    ></i>
    <span
      v-if="notify"
      class="h-3 w-3 inline-flex font-semibold items-center justify-center bg-red-600 absolute text-xs rounded-full text-white"
      style="font-size:7px;right:-4px"
      >{{ notify }}</span
    >
  </span>
</template>

<script>
export default {
  props: ["type", "notify", "rectangle", "large"],
  computed: {
    IconType() {
      let icon = null;
      if (this.type == "cog") {
        icon = "fas fa-cog";
      }
      if (this.type == "message") {
        icon = "fas fa-envelope";
      }
      if (this.type == "bell") {
        icon = "fas fa-bell";
      }
      if (this.type == "trash") {
        icon = "fas fa-trash";
      }
      if (this.type == "user") {
        icon = "fas fa-user";
      }
      if (this.type == "tag") {
        icon = "fas fa-tag";
      }
      if (this.type == "checkbox") {
        icon = "fa fa-check-square-o";
      }
      if (this.type == "paperclip") {
        icon = "fa fa-paperclip";
      }
      if (this.type == "file") {
        icon = "fa fa-file-text-o";
      }
      return icon;
    },
    borderRadius() {
      return this.rectangle ? "rounded-lg" : "rounded-full";
    },
    size() {
      return this.large ? "icon-size-lg" : "icon-size";
    },
  },
  // computed: {
  //   IconType() {
  //     let icon = null;
  //     if (this.type == "cog") {
  //       icon = "fas fa-cog";
  //     }
  //     if (this.type == "message") {
  //       icon = "fas fa-envelope";
  //     }
  //     if (this.type == "bell") {
  //       icon = "fas fa-bell";
  //     }
  //     return icon;
  //   },
  // },
};
</script>

<style scoped>
.icon-size-lg {
  font-size: 25px;
  line-height: 25px;
}
.icon-size {
  font-size: 10px;
  line-height: 10px;
}
</style>
