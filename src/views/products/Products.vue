<template>
  <div my-5 class="products">
    
    <v-container  class="my-5 text-center">
        <h1 class="subheading grey--text">Products</h1>
        <v-card flat class="pa-3" v-for="prod in projects" :key="prod.text" >
            <v-layout row wrap  class="pa-5">
                <v-flex xs12 md6>
                    <div class="caption grey--text  ">{{prod.title}}</div>
                    <div class="caption grey--text  ">{{prod.person}}</div>
                    

                </v-flex>
                <v-flex xs6 sm6 md2>
                    <div class="caption grey--text ">{{prod.title}}</div>
                    <div class="caption grey--text ">{{prod.person}}</div>


                </v-flex>
                <v-flex xs6 sm6 md2>
                    <div class="caption grey--text ">{{prod.title}}</div>
                    <div class="caption grey--text">{{prod.person}}</div>
                 

                </v-flex>
               

            </v-layout>
            <v-divider></v-divider>

        </v-card>

    </v-container>

  </div>
</template>

<script>
export default {
    data() {
        return {
            projects:[
                {title:"Desing a new website",person:"Net Stotka"},
                {title:"Code a new website",person:"Net ace"},
                {title:"Read a new website",person:"Net Acka"}

            ]
        }
    }

}
</script>

<style>

</style>