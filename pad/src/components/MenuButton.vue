<template>
  <v-btn color="white" @click="updateYossisTitle(text)">{{text}}</v-btn>
</template>

<script>
export default {
  name: "MenuButton",
  props: {
    text: {
      type: String,
      required: true
    },
    updateYossisTitle: {
      type: Function
    }
  }
};
</script>
