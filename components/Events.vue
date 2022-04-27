<!-- Please remove this file from your project -->
<template>
  <v-list>
    <v-list-item v-for="(item, i) in items" :key="i" :to="item.to" router exact>
      <v-list-item-content>
        <v-list-item-title v-text="item.name" />
      </v-list-item-content>
    </v-list-item>
  </v-list>
</template>

<script>
export default {
  name: 'Events',
  data () {
    return {
      items: [
        {
          name: 'controls.xxx',
          to: '/chat'
        }
      ]
    }
  }
}
</script>
