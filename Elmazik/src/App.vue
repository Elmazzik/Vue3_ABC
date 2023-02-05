<script>
export default {
  data() {},
  methods: {
    show: function () {
      let now = new Date();
      alert(now);
    },
  },
};
</script>

<template>
  <button @click="show">text</button>
</template>
