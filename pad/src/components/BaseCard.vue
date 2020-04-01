<template>
  <v-card height="100%">
    <v-card-title class='pink white--text'>{{title}}</v-card-title>
    <v-card-text>
      <slot></slot>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: "BaseCard",
  props: {
    title: {
      type: String,
      default: "כרטיס ללא שם"
    }
  }
};
</script>