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

    
  <v-expansion-panels class="my-5">
    <v-expansion-panel
    
    >
      <v-expansion-panel-header>Item</v-expansion-panel-header>
      <v-expansion-panel-content v-for="prod in myProjects" :key="prod.title">
        <div slot="header">{{prod.title}}</div>
        <v-card flat>
            <v-card-text class="px-4 grey--text">
                <div>{{prod.person}}</div>

            </v-card-text>
        </v-card>
      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>

      

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
    },
     computed: {
            myProjects() {
                return this.projects.filter(prod => {
                    return prod.person === "Net ace"
                })
            }
     }
}
</script>

<style>

</style>