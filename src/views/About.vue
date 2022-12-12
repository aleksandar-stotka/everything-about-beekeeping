<template>
  <div class="about">
    <v-container class="my-5">
      <v-layout row wrap>
        <v-flex xs12 md6>
          <v-btn outline block color="indigo">1</v-btn>

        </v-flex>
        <v-flex xs4 md2>
          <v-btn outlined  block class="primary">3</v-btn>

        </v-flex>
        <v-flex xs4 md2>
          <v-btn  outlined block class="primary">3</v-btn>

        </v-flex>
        <v-flex xs4 md2>
          <v-btn outline block class="primary">1</v-btn>

        </v-flex>

      </v-layout>

      <v-layout row wrap justify-space-around>
         <v-flex xs4 md3>
          <v-btn otline block>sas</v-btn>
         </v-flex>
         <v-flex xs4 md3>
          <v-btn otline block>sas</v-btn>
         </v-flex>
         
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import { ref } from 'vue';
export default {
  setup() {
    const ace = ref("ace")
    console.log(ace.value)


    return {ace}
  }
  
}
</script>
