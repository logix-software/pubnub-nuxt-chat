<template>
  <v-list>
    <v-list-item v-for="(item, i) in items" :key="i" :to="item.to" router exact>
      <v-list-item-action>
        <v-icon>{{ item.icon }}</v-icon>
      </v-list-item-action>
      <v-list-item-content>
        <v-list-item-title v-text="item.name" />
      </v-list-item-content>
    </v-list-item>
  </v-list>
</template>
<script>
export default {
  name: "Lists",
  data() {
    return {
      items: [
        {
          icon: "mdi-home",
          id: "",
          name: "Home",
          channelSubscribe: "",
          to: "/",
        },
      ],
    };
  },
};
</script>