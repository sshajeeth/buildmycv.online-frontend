<template>
  <v-app>
    <v-navigation-drawer v-model="sidebar" app>
      <v-list>
        <v-list-item v-for="item in menuItems" :key="item.title" :to="item.path">
          <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>{{ item.title }}</v-list-tile-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-toolbar app>
      <span class="hidden-sm-and-up">
        <v-app-bar-nav-icon @click="sidebar = !sidebar"></v-app-bar-nav-icon>
      </span>
      <v-toolbar-title>
        <router-link to="/" tag="span" style="cursor: pointer">{{ appTitle }}</router-link>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-xs-only">
        <v-btn
          class="mt-3 mx-2"
          text
          v-for="item in menuItems"
          :key="item.title"
          :to="item.path"
        >{{ item.title }}</v-btn>
        <v-btn
          id="login"
          class="mt-3 mx-2"
          shaped
          outlined
          light
          text
          color="primary"
          to="login"
        >Login</v-btn>
        <v-btn class="mx-2 mt-3" dark color="cyan darken-2" to="login">Create Free Resume</v-btn>
      </v-toolbar-items>
    </v-toolbar>

    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
//import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  data() {
    return {
      appTitle: "Build My CV",
      sidebar: false,
      menuItems: [
        { title: "Features", path: "/features" },
        { title: "Customers", path: "/customers" },
        { title: "Pricing", path: "/pricing" },
        { title: "About", path: "/about" }
      ]
    };
  }
};
</script>
<style>
.v-btn {
  border-radius: 30px !important;
}
#login {
  border-color: #0097a7;
  width: 200px;
}
</style>
