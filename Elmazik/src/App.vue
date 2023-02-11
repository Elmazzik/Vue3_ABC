<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      hidden: true,
    }
},
};
</script>

<template>
  <p v-if="!hidden">Lorem ipsum</p>
</template>
