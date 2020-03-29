<template>
  <v-layout row justify-space-around>
    <v-flex xs2>
      <v-layout column fill-height justify-space-around>
        <v-flex xs11>
          <Menu :onMenuBtnClick="this.updateYossi" />
        </v-flex>
      </v-layout>
    </v-flex>
    <v-flex xs9>
      <v-layout column fill-height justify-space-around>
        <v-flex xs6>
          <Yossi :title="currentYossi" />
        </v-flex>
        <v-flex xs4>
          <MoreInfo />
        </v-flex>
      </v-layout>
    </v-flex>
  </v-layout>
</template>

<script>
import Menu from "./Menu";
import Yossi from "./Yossi";
import MoreInfo from "./MoreInfo";

export default {
  name: "HomePage",
  data: function() {
    return {
      currentYossi: ""
    };
  },
  components: {
    Menu,
    Yossi,
    MoreInfo
  },
  methods: {
    updateYossi(newYossi) {
      this.currentYossi = newYossi;
    }
  }
};
</script>
