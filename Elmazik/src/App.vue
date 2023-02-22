<script>
export default {
  data() {
    return {
      checked: true,
    }
  },
  methods: {
    toggle: function () {
      this.checked = false;
    }
  }
}
</script>
<template>
      <input type="checkbox" v-model="checked">
      <p v-if="checked">{{ checked ? 'текст' : 'скрыто' }}</p>
</template>
<style>

</style>