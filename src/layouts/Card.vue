<template>
    <v-container class="position justify-center">
      <div class="mb-5 text-center">
        <h1 class="text-primary">Recents Blogs</h1>
      </div>
      <v-row class="pb-4 mt-4">
        <v-col v-for="n in 2" :key="n" cols="12" sm="12" md="12" :lg="col">
          <v-card
            class="mx-auto elevation-5 disp-card"
            :width="wdts"
            prepend-icon="mdi-delete">
            <template v-slot:title> My First Blog </template>
            <!-- Replace "Author" with {{ author }} to dynamically set the author's name -->
            <p class="ps-4">Author</p>
            <v-card-text> lorem ipsum hello my name is Furqan </v-card-text>
            <v-textarea
              variant="filled"
              auto-grow
              label="Reviews"
              rows="2"
              row-height="20"
            ></v-textarea>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script>
  export default {
    props: {
      author: String, // Prop to receive the author's name dynamically
      col: String,
      wdts: String,
    },
  };
  </script>
  
  <style>
  .position {
    margin-top: 140px;
  }
  
  /* Add shadow to cards using elevation classes */
  .elevation-5 {
    box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
  }
  .disp-card {
    background-color: white;
  }
  .disp-card:hover {
    background-color: bisque;
  
    border: 1px solid black;
  }
  </style>