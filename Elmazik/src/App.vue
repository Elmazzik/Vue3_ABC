<script>
export default {
  data() {
    return {
      language: '',
      visible: false,
      visible1: false,
      visible2: false,
    }
  },
  methods: {
    one() {
      this.visible = true;
    },
    two() {
      this.visible1 = true;
    },
    three() {
      this.visible2 = true;
    }
  }
}
</script>
<template>
      <input type="radio" v-model="language" value="Русский" @click="first">
      <p>Turkish</p>
      <p></p>
      <input type="radio" v-model="language" value="Английский" @click="second">
      <p>Ukrainian</p>
      <p></p>
      <input type="radio" v-model="language" value="Крымскотатарский" @click="third">
      <p></p>
      <p>Russian</p>
      <p v-if="visible">Привет, будешь чай?</p>
      <p v-else-if="visible1">Hi, do you want some tea?</p>
      <p v-else-if="visible2">Селям, чай ичеджен? </p>

</template>
<style>

</style>