<script>
export default {
  data() {
    return {
      attr: "./public/kotik.jpg",
    };
  },
};
</script>

<template>
  <img :src="attr" class="cat" />
</template>
