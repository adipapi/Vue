<template>
    <v-card class="mx-auto" max-width="400" color="red">
      <v-card-title class="title">{{title}}</v-card-title>
      <v-card-text>hello</v-card-text>
    </v-card>
</template>

<script>
/* eslint-disable */
export default {
  name: "Card",
  data(data) {
    return {
      title: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<style scoped>
.title {
  background: palevioletred;
}
</style>
