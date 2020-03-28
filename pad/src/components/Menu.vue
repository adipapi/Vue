<template>
    <Card title='תפריט' >
      <v-btn-toggle borderless slot="card-content" color="blue" class="d-flex flex-column">
        <MenuButton text="דואר נכנס" />
        <MenuButton text="דואר יוצא" />
      </v-btn-toggle>
    </Card>
</template>

<script>
import Card from './Card';
import MenuButton from './MenuButton';
export default {
  name: 'Menu',
  components: {
    Card,
    MenuButton
  }
};
</script>
