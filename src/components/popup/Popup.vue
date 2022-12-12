<template>
  <div class="text-center">
    <v-dialog
      v-model="dialog"
      width="500"
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="success"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Click Me
        </v-btn>
      </template>

      <v-card>
        <v-card-title
          class="headline grey lighten-2"
          primary-title
        >
          Privacy Policy
        </v-card-title>

        <v-card-text>
          <v-form class="px-3">
            <v-text-field label="Title"  v-model="title"></v-text-field>
            <v-textarea label="Information" v-model="content"></v-textarea>
             <v-btn @click="submit" class="success mx-3" text>Add Project</v-btn>
          </v-form> 
        </v-card-text>

        <v-divider></v-divider>

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="success"
            text
            @click="dialog = false"
          >
            I accept
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
      title: "",
      content:''
    }
  },
  methods: {
    submit() {
      console.log(this.title,this.content)
    }
  }

}
</script>

<style>

</style>