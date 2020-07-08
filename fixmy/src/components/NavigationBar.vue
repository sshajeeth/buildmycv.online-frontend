<template>
  <v-app app>
    
        <v-chip
          
          color="grey lighten-4"
          light
          class="mx-1 mt-2 ma-6"
          v-for="item in menuItems"
          :key="item.title"
          :to="item.path"
        >{{ item.title }}</v-chip>
      
  </v-app>
</template>

<script>
//import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  data() {
    return {
      appTitle: "Awesome App",
      sidebar: false,
      menuItems: [
        { title: "Features", path: "/home", icon: "home" },
        { title: "Customers", path: "/signup", icon: "face" },
        { title: "Pricing", path: "/signin", icon: "lock_open" },
        { title: "Login", path: "/login", icon: "lock_open" },
        { title: "Create Your Resume", path: "/login", icon: "lock_open" }
      ]
    };
  }
};
</script>
<style>
</style>
