<template>
  <BaseCard title="תפריט">
    <v-btn-toggle borderless color="blue" class="d-flex flex-column">
      <MenuButton text="דואר נכנס" @changePageTitle="updateCurrentPageTitle($event)" />
      <MenuButton text="דואר יוצא" @changePageTitle="updateCurrentPageTitle($event)" />
      <MenuButton text="דואר זבל" @changePageTitle="updateCurrentPageTitle($event)" />
    </v-btn-toggle>
  </BaseCard>
</template>

<script>
import BaseCard from "./BaseCard";
import MenuButton from "./MenuButton";
export default {
  name: "Menu",
  components: {
    BaseCard,
    MenuButton
  },
  methods: {
    updateCurrentPageTitle(newTitle) {
      this.$emit('updateCurrentPageTitle',newTitle)
    }
  }
};
</script>
