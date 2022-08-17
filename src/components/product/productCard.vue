<template>
  <v-card elevation="10" outlined max-width="800" class="mx-auto my-5">
    <v-card-title>test</v-card-title>
    <v-card-text
      >Lorem ipsum dolor sit amet consectetur adipisicing elit.</v-card-text
    >
    <v-divider class="mx-2"></v-divider>
    <v-card-text>
        Packaging options
      <v-chip-group active-class="primary--text">
        <v-chip>1 for $4</v-chip>
        <v-chip>1 for $4</v-chip>
        <v-chip>1 for $4</v-chip>
        <v-chip>1 for $4</v-chip>
      </v-chip-group>
    </v-card-text>
    <v-card-actions>
      <v-btn color="primary"> Add to cart </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    items: ["Foo", "Bar", "Fizz", "Buzz"],
  }),
};
</script>

<style></style>
