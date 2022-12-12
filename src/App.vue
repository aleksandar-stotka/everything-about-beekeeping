<template>
  <v-app class="grey lighten-4">
    <Nav/>
  
   <v-content>
    <router-view></router-view>
   </v-content>
  </v-app>
</template>

<script>
import Nav from '@/components/Navbar.vue/Nav'
export default {

  name: 'App',
  components: {
    Nav
  },

};
</script>
