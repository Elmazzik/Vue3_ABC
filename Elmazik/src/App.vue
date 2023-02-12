<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      items: [1, 2, 3, 4, 5],
    }
  },
}
</script>

<template>
  <p v-for="elem in items">{{ elem }}</p>
    <div v-for="elem in items">{{ elem ** 2 }}</div>
    <ul>
      <li v-for="elem in items">{{ elem }}</li>
    </ul>
</template>
