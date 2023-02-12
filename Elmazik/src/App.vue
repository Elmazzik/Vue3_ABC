<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
    }
  }
}
</script>

<template>
    <p v-for="num in 30">
      {{ num }}
    </p>
</template>
