<template>
  <div class="Carrito">
    <ShoppingCart />
  </div>
</template>

<script>
import ShoppingCart from '~/components/partials/shopping/ShoppingCart.vue'
export default {
  name: 'Carrito',
  components: { ShoppingCart },
}
</script>
