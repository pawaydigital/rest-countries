<template>
  <svg class="m-1" width="30px" height="25px">
    <path :fill="color" :d="icon" />
  </svg>
  <span v-if="text" class="m-1">{{ text }}</span>
</template>

<script>
export default {
  props: {
    icon: String,
    color: String,
    text: {
      type: String,
      default: "",
    },
  },
};
</script>
