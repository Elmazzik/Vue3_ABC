<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      cost: 200,
      amount: 3,
    }
  },
  methods: {
      change: function (i) {
      this.amount = this.amount + 1;
      this.cost = this.cost + 100;
      },
    },
  computed: {
    price: function () {
      return this.cost * this.amount;
    },
  },
};
</script>

<template>
  <p>{{ cost }}</p>
  <p>{{ amount }}</p>
  <p>{{ price }}</p>
  <button @click='change(text)'>change</button>
</template>
