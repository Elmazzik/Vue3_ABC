<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      products: [
        {
          id: 1,
          name: 'product1',
        },
        {
          id: 2,
          name: 'product2',
        },
        {
          id: 3,
          name: 'product3',
        },
      ]
    }
  }
}
</script>

<template>
<ul>
    <li v-for="product in products" :key="product.name">
		{{ product.name }}
    </li>
</ul>
</template>
