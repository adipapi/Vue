<template>
  <v-btn color="white" @click="onMenuBtnClick(text)">{{text}}</v-btn>
</template>

<script>
export default {
  name: "MenuButton",
  props: {
    text: {
      type: String,
      required: true
    },
    onMenuBtnClick: {
      type: Function
    }
  }
};
</script>
