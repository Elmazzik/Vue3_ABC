<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      visible: true,
    }
},
  methods: {
    hide: function () {
      this.visible = false;
    },
    nothide: function () {
      this.visible = true;
    }
  }
};
</script>

<template>
  <button @click="hide" v-if="visible">hide</button>
  <button @click="nothide" v-if="!visible">not hide</button>
  <p v-if="visible">Hello!</p>
</template>
