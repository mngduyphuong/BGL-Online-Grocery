<template>
  <div class="pa-5">
    <productTable></productTable>
  </div>
</template>

<script>
import productTable from '@/components/product/productTable.vue'

export default {
  name: "Home",
  components: {
      productTable
  },
};
</script>