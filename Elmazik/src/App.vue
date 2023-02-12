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
  <p v-show="isAuth">+++</p>
  <button @click="toggle">скрыть</button>
</template>
