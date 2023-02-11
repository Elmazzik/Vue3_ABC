<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      visible: true,
    }
},
  methods: {
    toggle: function () {
      this.visible = !this.visible;
    }
  }
};
</script>

<template>
  <button @click="toggle">first</button>
  <p v-if="visible">one</p>
</template>
