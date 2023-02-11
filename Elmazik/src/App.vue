<script>
import { normalizeProps } from 'vue';

export default {
  data() { },
  methods: {
    show: function (i) {
      alert(i ** 2);
    },
  },
};
</script>

<template>
  <button @click="show('2')">2</button>
  <button @click="show('3')">3</button>
</template>
