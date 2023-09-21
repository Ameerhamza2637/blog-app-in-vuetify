<template>
    <v-app>
      <Navbar title="Guest Dashboard"/>
      <Card col="6" wdts="400px" />
    </v-app>
    <Sidebar />
  </template>
  
  <script>
  //  import Sidebar from '@/layouts/Sidebar.vue'
  import Navbar from "@/layouts/Navbar.vue";
  //import Sidebar from "@/layouts/Sidebar.vue";
  import Card from "@/layouts/Card.vue";
  export default {
    components: {
    //  Sidebar,
      Navbar,
      Card,
    },
  };
  </script>
  
  <style>
  
  
  </style>