<template>
    <div class="create">
     

        <v-container class="my-5 text-center" >
            <h1 class="subheading grey--text">Create</h1>

            <v-layout row wrap>
                <v-flex xs12 sm6 md4 lg3 v-for="prod in projects" :key="prod.text">
                    <v-card text class="text-center ma-3">
                        <v-responsive class="pt-4">
                            <v-avatar size="100">
                                <img :src="prod.avatar" />
                            </v-avatar>
                        </v-responsive>
                        <v-card-text>
                            <div class="subheading">{{prod.title}}</div>
                            <div class="grey--text">{{prod.person}}</div>
                        </v-card-text>
                      
                            <v-btn block text smalls color="grey" >add</v-btn>
                       

                    </v-card>

                </v-flex>

            </v-layout>

        </v-container>
    </div>
  
</template>

<script>
export default {
    data() {
        return {
            projects:[
                {title:"Desing a new website",person:"Net Stotka",avatar:'/logo.png'},
                {title:"Code a new website",person:"Net ace",avatar:'/logo.png'},
                {title:"Read a new website",person:"Net Acka",avatar:'/logo.png'},
                {title:"Read a new website",person:"Net Acka",avatar:'/logo.png'},
                {title:"Read a new website",person:"Net Acka",avatar:'/logo.png'}

            ]
        }
    }

}
</script>

<style>

</style>