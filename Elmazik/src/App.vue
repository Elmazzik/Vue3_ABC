<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      age: 26,
    }
  }
};
</script>

<template>
<p v-if="age < 18">подросток</p>
<p v-else-if="age >= 19 && age <= 25">молодой человек</p>
<p v-else>мужчина</p>
</template>
