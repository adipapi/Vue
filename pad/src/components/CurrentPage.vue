<template>
  <BaseCard :title="title" />
</template>

<script>
import BaseCard from "./BaseCard";

export default {
  name: "CurrentPage",
  components: {
    BaseCard
  },
  props: {
    title: {
      type: String
    }
  }
};
</script>
