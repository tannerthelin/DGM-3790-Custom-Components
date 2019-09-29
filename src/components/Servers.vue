<template>
  <v-card
    class="mx-auto"
    max-width="400"
    width="undefined"
    tile
  >
    <v-list rounded>
      <v-subheader>SERVERS</v-subheader>
      <v-list-item-group v-model="item" color="primary">
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
        >
          <v-list-item-icon>
            <v-icon v-text="item.icon"></v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title v-text="item.text"></v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      item: 1,
      items: [
        { text: 'Server 01', icon: 'mdi-database-check' },
        { text: 'Server 02', icon: 'mdi-database-check' },
        { text: 'Server 03', icon: 'mdi-database-remove' },
      ],
    }),
  }
</script>