<template>
  <v-app>
    <v-main>
      <v-container>
        <v-card><v-icon>fas fa-home</v-icon></v-card>
      </v-container>
    </v-main>
  </v-app>
</template>
<script>
export default {
  layout: "default",
  name: "PageIndex",
  head: () => ({
    titleTemplate: "%s",
  }),
  created() {
    this.$store.dispatch("app/loaded");
  },
};
</script>
