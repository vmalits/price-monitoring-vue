<template>
  <v-app id="main">
    <nav-bar ref="navbar"></nav-bar>

    <app-header
      @toggle-drawer="$refs.navbar.drawer = !$refs.navbar.drawer"
    ></app-header>

    <v-main>
      <v-container fluid>
        <v-spacer />
        <router-view></router-view>
      </v-container>
    </v-main>

    <app-footer></app-footer>
  </v-app>
</template>

<script>
import Footer from "@/components/Footer";
import Header from "@/components/Header";
import NavBar from "@/components/NavBar";

export default {
  name: "App",

  components: {
    "nav-bar": NavBar,
    "app-header": Header,
    "app-footer": Footer
  },

  data: () => ({})
};
</script>
