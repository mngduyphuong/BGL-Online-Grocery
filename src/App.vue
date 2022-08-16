<template>
  <v-app>
    <nav-bar></nav-bar>
    <v-main>
      <v-container fluid>
        <router-view></router-view>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import navBar from '@/components/nav/navBar.vue'

export default {
  name: "App",
 components: {
      navBar
  },
};
</script>
