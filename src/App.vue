<template>
  <v-app style="background-color: lightgrey;">
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
