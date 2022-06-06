<template>
  <v-container class="container">
    <v-row class="login-row" justify="center" align="center">
      <login-card-view />
    </v-row>
  </v-container>
</template>

<script>
import { defineComponent } from "vue";
import LoginCardView from "../components/LoginCard.vue";

export default defineComponent({
  name: "HomeView",

  components: {
    LoginCardView,
  },
});
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
.container {
  width: 100%;
  height: 100vh;
  background-color: cornsilk;
  margin: 0 !important;
  padding: 0 !important;
  max-width: none;
}

.login-row {
  height: 100vh;
}
</style>
