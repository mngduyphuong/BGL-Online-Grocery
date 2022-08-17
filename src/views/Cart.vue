<template>
  <div>
    <cart-list></cart-list>
  </div>
</template>

<script>
import cartList from "@/components/cart/cartList.vue";
export default {
  name: "Cart",
  components: {
    cartList,
  },
};
</script>
