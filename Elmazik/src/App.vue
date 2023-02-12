<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      products: [
        {
          name: 'product1',
          price: 100,
          quantity: 5
        },
        {
          name: 'product2',
          price: 200,
          quantity: 4
        },
        {
          name: 'product3',
          price: 300,
          quantity: 3
        },
      ]
    }
  }
}
</script>

<template>
    <table v-for="product in products">
    {{ product.name }}
    {{ product.price }}
    {{ product.quantity }}
    </table>
</template>
