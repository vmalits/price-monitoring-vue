<template>
  <v-navigation-drawer v-model="drawer" app>
    <v-list dense>
      <v-list-item-avatar>
        <img alt="Vue logo" src="../assets/logo.png" />
      </v-list-item-avatar>

      <v-list-item link exact :to="{ name: 'Home' }">
        <v-list-item-action>
          <v-icon>mdi-home</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title>Home</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-list-item link exact :to="{ name: 'About' }">
        <v-list-item-action>
          <v-icon>mdi-information</v-icon>
        </v-list-item-action>
        <v-list-item-content>
          <v-list-item-title>About</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "NavBar",
  data: () => {
    return {
      drawer: true
    };
  }
};
</script>

<style scoped></style>
