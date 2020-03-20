<template>
  <v-layout row ma-5>
    <v-flex xs4 sm3 md2 ml-5 pr-3>
      <Card v-bind:props="Menu" />
    </v-flex>
    <v-flex>
      <v-layout column fill-height>
        <v-flex>
          <Card v-bind:props="Yossi" />
        </v-flex>
        <v-flex mt-5>
          <Card v-bind:props="MoreInfo" />
        </v-flex>
      </v-layout>
    </v-flex>
  </v-layout>
</template>

<script>
import Card from './Card';

export default {
  name: 'HomePage',
  components: {
    Card
  },
  data() {
    return {
      Menu: { title: 'תפריט' },
      Yossi: { title: 'יוסי' },
      MoreInfo: { title: 'מידע נוסף' }
    };
  }
};
</script>
