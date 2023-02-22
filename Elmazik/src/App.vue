<script>
export default {
  data() {
    return {
      arr: [],
    }
  }
}
</script>
<template>
  <input type="checkbox" v-model="arr" value="Русский">
  <label>Русский</label>
  <br>
  <input type="checkbox" v-model="arr" value="Английский">
  <label>Английский</label>
  <br>
  <input type="checkbox" v-model="arr" value="Крымскотатарский">
  <label>Крымскотатарский</label>
  <ul>
  <li v-for="elem in arr">{{ elem }}</li>
  </ul>
</template>
<style>

</style>