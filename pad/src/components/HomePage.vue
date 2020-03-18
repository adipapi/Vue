<template>
  <div>
    <p>Hello</p>
    <div>
      <Card />
    </div>
    <div class="d-flex pa-2">
      <Card />
      <Card />
    </div>
  </div>
</template>

<script>
/* eslint-disable */
import Card from "./Card";

export default {
  name: "HomePage",
  components: {
    Card
  }
};
</script>
