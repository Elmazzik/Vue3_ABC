<script>
export default {
  data() {
    return {
      selected: 'Симферополь',
    }
  },
  methods: {
  }
}
</script>
<template>
      <p>В каком городе ты живешь?</p>
      <select v-model="selected">
        <option>Симферополь</option>
        <option>Нью-Йорк</option>
        <option>Сыктывкар</option>
      </select>
      <p>{{ selected }}</p>
</template>
<style>

</style>