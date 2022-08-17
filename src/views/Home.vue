<template>
  <div class="text-center">
    <div class="text-h4 primary--text">Welcome to BGL Online Grocery Shop </div>
    <div class="text-subtitle-1">More than a Software</div>
    <v-row>
      <v-col md="4">
         <product-card></product-card>
      </v-col>
      <v-col md="4">
         <product-card></product-card>
      </v-col>
      <v-col md="4">
         <product-card></product-card>
      </v-col>
      <v-col md="4">
         <product-card></product-card>
      </v-col>
    </v-row>
   
    
  </div>
</template>

<script>
import productCard from '@/components/product/productCard.vue'

export default {
  name: "Home",
  components: {
      productCard
  },
};
</script>
