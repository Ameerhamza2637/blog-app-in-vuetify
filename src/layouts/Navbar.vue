<template>
     <div class="navs">
        <v-app-bar app>
        <v-app-bar-nav-icon @click="toggleSidebar"></v-app-bar-nav-icon>
        <v-toolbar-title>{{ title }}</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn text @click="logout">Logout</v-btn>
        </v-app-bar>
     </div>
  </template>
  
  <script>
  export default {
    props:
    {
        title: String,
    },
    methods: {
      toggleSidebar() {
        // You can implement the logic to toggle the sidebar here
      },
      logout() {
        // Implement your logout logic here
      }
    }
  };
  </script>
  
  <style scoped>
  /* Add any custom styles for your Navbar here */
  
  /* Media query for screens smaller than 600px */
  @media (max-width: 600px) {
    .toggle-icon {
      display: inline-block; /* Show the hamburger icon */
    }
    .title {
      display: none; /* Hide the title */
    }
    .logout-btn {
      font-size: 12px; /* Reduce the font size of the Logout button */
    }
  }
  .navs{
    min-height: 0dvh;
    min-height: 0vh;
  }
 
  
  /* Add more media queries and styles as needed for other screen sizes */
  </style>
  