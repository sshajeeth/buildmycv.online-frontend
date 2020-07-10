<template>
  <v-app>
    <v-content>
      <NavigationDrawer/>
      
    </v-content>
    <v-content>
      <v-container>
        <v-card shaped min-height="300" max-height="300" max-width="300" min-width="300" class="elevation-12">
          <v-card-text>
          <v-icon style="margin-top:30px;" x-large>add</v-icon>
          </v-card-text>
        </v-card>
      </v-container>
    </v-content>
  </v-app>

  
</template>

<script>
// @ is an alias to /src
import NavigationDrawer from '@/components/NavigationDrawer.vue'

export default {
  
  components: {
    NavigationDrawer
  }
}
</script>
