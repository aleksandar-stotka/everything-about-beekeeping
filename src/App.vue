<template>
  <v-app style="background-color: lightgrey;">
    <Nav/>
  
   <v-main>
    <router-view></router-view>
   </v-main>
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
