<template>
  <span v-if="regular">
    <i
      class="p-2 rounded-full border border-gray-700 fas fa-check bg-grayish text-gray-700"
      :class="iconSize ? 'icon-size-sm' : 'icon-size'"
    ></i>
  </span>
  <span v-if="solid">
    <i
      class="p-2 rounded-full fas fa-check bg-primary text-white"
      :class="iconSize ? 'icon-size-sm' : 'icon-size'"
    ></i>
  </span>
</template>

<script>
export default {
  props: ["solid", "regular", "small"],
  computed: {
    iconSize() {
      let icon_size = "";
      if (this.small) {
        icon_size = "icon-size-sm";
      }
      return icon_size;
    },
  },
};
</script>

<style scoped>
.icon-size-sm {
  font-size: 8px;
  line-height: 8px;
}
</style>
