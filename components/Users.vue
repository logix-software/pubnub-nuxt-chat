<!-- Please remove this file from your project -->
<template>
  <v-list>
    <v-list-item v-for="(user, i) in users" :key="i" :to="user.to" router exact>
      <v-list-item-action>
        <v-icon>{{ user.icon }}</v-icon>
      </v-list-item-action>
      <v-list-item-content>
        <v-list-item-title v-text="user.name" />
      </v-list-item-content>
    </v-list-item>
  </v-list>
</template>

<script>
export default {
  name: "Users",
  data () {
    return {
      users: [
        {
          icon: 'mdi-account',
          id: '19876',
          name: 'User',
          channelSubscribe: 'controls.xxx.19876',
          to: '/chat?id=19876'
        }
      ]
    }
  }
};
</script>
