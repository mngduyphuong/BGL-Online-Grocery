<template>
    <v-card class="mx-auto ma-4" max-width="300">
      <v-list>
        <v-list-item
          v-for="i in 5"
          :key="i"
        >
          <v-list-item-content>
            <v-list-item-title>
              Item name x14: $120
            </v-list-item-title>
            <v-list-item-subtitle>
              Subtitle 1: $10
            </v-list-item-subtitle>
            <v-list-item-subtitle>
              Subtitle 2: $10
            </v-list-item-subtitle>
            <v-list-item-subtitle>
              Subtitle 3: $10
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-divider></v-divider>
        <v-list-item><h3>Total: $144</h3></v-list-item>
      </v-list>
      
    </v-card>
</template>

<script>
export default {

}
</script>

<style>

</style>