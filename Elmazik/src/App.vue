<script>
export default {
  data() {
    return {
      obj: { a: 1, b: 2, c: 3 },
    };
  },
};
</script>

<template>
  {{ obj.c + obj.b + obj.a }}
</template>
