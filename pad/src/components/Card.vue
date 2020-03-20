<template>
  <v-card height='100%'>
    <v-card-title class='pink white--text'> {{props.title}} </v-card-title>
    <v-card-text></v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'Card',
  props: ['props']
};
</script>
