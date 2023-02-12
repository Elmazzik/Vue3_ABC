<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      visible: [ true, true, true]
    }
},
  methods: {
    toggle: function (i) {
      this.visible[i] = !this.visible[i];
    }
  }
};
</script>

<template>
  <button @click="toggle(1)">first</button>
  <p v-if="visible[1]">one</p>
  <button @click="toggle(2)">second</button>
  <p v-if="visible[2]">two</p>
  <button @click="toggle(3)">third</button>
  <p v-if="visible[3]">three</p>
</template>
