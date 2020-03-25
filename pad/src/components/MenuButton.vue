<template>
    <v-btn>{{text}}</v-btn>
</template>

<script>

export default {
  name: 'MenuButton',
    props: {
    text: 
    {
        type: String,
        required: true
    }
  }
};
</script>
