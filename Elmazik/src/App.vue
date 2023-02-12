<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      arr: ['x', 'y', 'z'],
    }
  },
}
</script>

<template>
    <ul>
      <li v-for="(elem, key) in arr">{{ key + 1 }} {{ elem }}</li>
    </ul>
</template>
