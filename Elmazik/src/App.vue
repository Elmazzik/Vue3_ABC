<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      arr: ['a', 'b', 'c'],
    }
  },
  methods: {
    add: function () {
      this.arr.push('xxx');
    }
  }
}
</script>

<template>
  <p v-for="elem in arr">
    {{ elem }}
  </p>
  <button @click="add">add</button>
</template>
