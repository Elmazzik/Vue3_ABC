<script>
export default {
  data() {
    return {
      isDisabled: true,
      isDisabled1: true,
      checked: false,
    }
  },
  methods: {
    cat: function () {
      this.isDisabled = false;
    },
    tea: function () {
      this.isDisabled1 = false;
    },
  }
}
</script>
<template>
  <input type="text" class="text-field__input"  v-bind:disabled="isDisabled">
  <br>
  <button @click="cat">cat</button>
  <br>
  <br>
  <br>
  <input type="text" class="text-field__input" v-bind:disabled="isDisabled1">
  <br>
  <input type="checkbox" v-model="checked" @click="tea">
  <button @click="tea">tea</button> 
</template>
<style>

</style>