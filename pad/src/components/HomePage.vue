<template>
  <v-layout row justify-space-around>
    <v-flex xs2>
      <v-layout column fill-height justify-space-around>
        <v-flex xs11>
          <Menu @updateCurrentPageTitle="currentPageTitle = $event" />
        </v-flex>
      </v-layout>
    </v-flex>
    <v-flex xs9>
      <v-layout column fill-height justify-space-around v-if="currentPageTitle !== 'דואר זבל'">
        <v-flex xs6>
          <CurrentPage :title="currentPageTitle" />
        </v-flex>
        <v-flex xs4>
          <MoreInfo />
        </v-flex>
      </v-layout>
      <v-layout column fill-height justify-space-around v-else>
        <v-flex xs11>
          <CurrentPage :title="currentPageTitle" />
        </v-flex>
      </v-layout>
    </v-flex>
  </v-layout>
</template>

<script>
import Menu from "./Menu";
import CurrentPage from "./CurrentPage";
import MoreInfo from "./MoreInfo";

export default {
  name: "HomePage",
  data: function() {
    return {
      currentPageTitle: ""
    };
  },
  components: {
    Menu,
    CurrentPage,
    MoreInfo
  }
};
</script>
