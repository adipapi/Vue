<template>
  <v-layout row justify-space-around>
    <v-flex xs2>
      <v-layout column fill-height justify-space-around>
        <v-flex xs11>
          <Menu :updateYossisTitle="this.updateYossisTitle" />
        </v-flex>
      </v-layout>
    </v-flex>
    <v-flex xs9>
      <v-layout column fill-height justify-space-around v-if="currentYossiTitle !== 'דואר זבל'">
        <v-flex xs6>
          <Yossi :title="currentYossiTitle" />
        </v-flex>
        <v-flex xs4>
          <MoreInfo />
        </v-flex>
      </v-layout>
      <v-layout column fill-height justify-space-around v-else>
        <v-flex xs11>
          <Yossi :title="currentYossiTitle" />
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
      currentYossiTitle: ""
    };
  },
  components: {
    Menu,
    Yossi,
    MoreInfo
  },
  methods: {
    updateYossisTitle(newTitle) {
      this.currentYossiTitle = newTitle;
    }
  }
};
</script>
