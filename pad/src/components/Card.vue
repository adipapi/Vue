<template>
  <v-card height="100%">
    <v-card-title class="title">{{title}}</v-card-title>
    <v-card-text>
      <slot name="card-content"></slot>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: "Card",
  props: {
    title: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.title {
  color: white;
  background: deeppink;
  height: 3em;
}
</style>
