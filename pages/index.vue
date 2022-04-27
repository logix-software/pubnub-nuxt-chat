<template>
  <v-app dark>
    <v-navigation-drawer v-model="drawer" fixed app>
      <Lists />
    </v-navigation-drawer>
    <v-app-bar :clipped-left="clipped" fixed app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
    </v-app-bar>
    <v-main>
      <v-container>
        <Events />
      </v-container>
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      drawer: false,
      title: "Chat Pubnub"
    };
  },
};
</script>
