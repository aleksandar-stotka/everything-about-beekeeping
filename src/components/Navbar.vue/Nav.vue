<template>
  <nav>
    <v-app-bar flat>
      <v-toolbar-title class="text-uppercase grey--text">
        <span class="font-weight-light">Toto</span>
        <span>Bee</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text color="accent">
        <span>Sign Out</span>
        <v-icon dark right> mdi-arrow-up-bold-box-outline </v-icon>
      </v-btn>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute temporary>
        <v-card
    class="mx-auto"
    max-width="500"
  >
    <v-list>
      <v-list-item-group v-model="model">
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
     
    </v-navigation-drawer>
    <v-btn color="pink" dark @click.stop="drawer = !drawer"> Toggle </v-btn>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      drawer: null,
      items: [
        {
          icon: 'mdi-inbox',
          text: 'Inbox',
        },
        {
          icon: 'mdi-star',
          text: 'Star',
        },
        {
          icon: 'mdi-send',
          text: 'Send',
        },
        {
          icon: 'mdi-email-open',
          text: 'Drafts',
        },
      ],
      model: 1,
    }
  },
};
</script>

<style></style>
