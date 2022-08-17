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

      <!-- Normal breakpoint nav bar -->
      <v-tabs centered class="hidden-sm-and-down">
        <v-tab link to="/"> Home </v-tab>
        <v-tab link to="/products"> Products </v-tab>
        <v-spacer></v-spacer>
        <v-tab link to="/cart" class="float-right">
          <span>Cart</span>
          <v-icon class="ml-2">mdi-cart-minus</v-icon></v-tab
        >
      </v-tabs>

      <!-- Small breakpoint toggle nav bar -->
      <v-spacer class="hidden-sm-and-up"></v-spacer>
      <v-app-bar-nav-icon
        @click="drawer = !drawer"
        left
        class="hidden-sm-and-up"
      ></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" temporary right app>
      <v-list nav>
        <v-list-item link to="/">
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/products">
          <v-list-item-content>
            <v-list-item-title>Products</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/cart">
          <v-list-item-content>
            <v-list-item-title>Cart</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
  }),
};
</script>

<style></style>
