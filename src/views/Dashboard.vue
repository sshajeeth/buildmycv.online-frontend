<template>
  <v-app>
    <v-content>
      <NavigationDrawer/>
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
