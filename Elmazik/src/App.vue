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
  <button @click="toggle(1)">{{ visible[1] ? 'hide' : 'show' }}</button>
  <p v-if="visible[1]">one</p>
  <button @click="toggle(2)">{{ visible[2] ? 'hide' : 'show' }}</button>
  <p v-if="visible[2]">two</p>
  <button @click="toggle(3)">{{ visible[3] ? 'hide' : 'show' }}</button>
  <p v-if="visible[3]">three</p>
</template>
