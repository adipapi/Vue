<template>
  <Card :title="title" />
</template>

<script>
import Card from "./Card";

export default {
  name: "Yossi",
  components: {
    Card
  },
  props: ["title"]
};
</script>
