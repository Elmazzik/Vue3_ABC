<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      num: 5,
    }
  }
};
</script>

<template>
  <p v-if="num === 1">monday</p>
  <p v-if="num === 2">tuesday</p>
  <p v-if="num === 3">wednesday</p>
  <p v-if="num === 4">thursday</p>
  <p v-if="num === 5">friday</p>
  <p v-if="num === 6">saturday</p>
  <p v-if="num === 7">sunday</p>
</template>
