<script>
export default {
  data() {
    return {
      arr: ["x", "y", "z"],
    };
  },
};
</script>

<template>
  {{ arr[0] }}
  <br />
  {{ arr[1] }}
  <br />
  {{ arr[2] }}
</template>
