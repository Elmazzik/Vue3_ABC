<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      isAuth: true,
}
},
methods: {
    toggle: function () {
    this.isAuth = !this.isAuth;
    }
  }
};
</script>

<template>
  <template v-if="isAuth">
    <p>+++</p>
    <p>+++</p>
    <p>+++</p>
  </template>
  <button @click="toggle">скрыть</button>
</template>
