<template>
  <v-footer color="deep-purple" app>
    <span class="white--text"
      >Copyright &copy; Price Monitoring {{ currentYear }}</span
    >
  </v-footer>
</template>

<script>
export default {
  name: "Footer",
  computed: {
    currentYear() {
      return new Date().getFullYear();
    }
  }
};
</script>

<style scoped></style>
