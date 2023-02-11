<script>
import { normalizeProps } from 'vue';

export default {
  data() {},
  methods: {
    elmaz: function (i) {
      alert("Привет!");
      return false;
  },
},
};
</script>

<template>
  <a href="elmaz.html" v-on:click.prevent><p>Тыкай сюда</p></a>
  <button v-on:click.once="elmaz">button</button>
</template>
