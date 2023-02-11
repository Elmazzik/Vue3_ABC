<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      text: 'Elmazik',
    }
  },
  methods: {
      change: function (i) {
        this.text = this.text + " " + "text...";
      },
      achange: function (i) {
        this.text = "text...";
      },
    },
};
</script>

<template>
  {{ text }}
  <button @click='change(text)'>change</button>
  <button @click='achange(text)'>achange</button>
</template>
