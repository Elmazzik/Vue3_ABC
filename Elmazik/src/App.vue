<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      visible: true,
    }
},
};
</script>

<template>
<p v-if="visible">Lorem ipsum</p>
</template>
