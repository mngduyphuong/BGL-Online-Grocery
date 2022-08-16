<template>
  <div>
    <v-app-bar app color="primary" dark>
        <!-- Logo -->
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          src="@/assets/bgl.jpg"
          width="50"
        />
      </div>

      <v-tabs centered class="hidden-sm-and-down">
        <v-tab v-for="link in links" :key="link">
          {{ link }}
        </v-tab>
      </v-tabs>
      <v-btn plain class="hidden-sm-and-down">
        <span>Cart</span>
        <v-icon class="ml-2">mdi-cart-minus</v-icon>
      </v-btn>


      <v-spacer class="hidden-sm-and-up"></v-spacer>
      <v-app-bar-nav-icon
        @click="drawer = !drawer"
        left
        class="hidden-sm-and-up"
      ></v-app-bar-nav-icon>
      
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" temporary bottom app>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    links: ["Dashboard", "Messages", "Profile", "Updates"],
  }),
};
</script>

<style></style>
