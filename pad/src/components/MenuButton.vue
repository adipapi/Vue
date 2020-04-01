<template>
  <v-btn color="white" @click="changePageTitle()">{{text}}</v-btn>
</template>

<script>
export default {
  name: "MenuButton",
  props: {
    text: {
      type: String,
      default: "כפתור ללא שם"
    }
  },
  methods: {
    changePageTitle() {
      this.$emit('changePageTitle',this.text)
    }
  }
};
</script>
