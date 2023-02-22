<script>
export default {
  data() {
    return {
      cat: ['karamelka', 'korzhik', 'compot'],
      tea: '',
    }
  },
  methods: {
    addcat: function () {
      this.cat.unshift(this.cat);
    }
  }
}
</script>
<template>
  <ul class="styled">
  <li v-for="(item, index) in 
  			cat" :key="index">
      {{ item }}
  </li>
  </ul>
  <input class="text-field__input" v-model="bmteaw">
  <br>
  <button @click="addcat">Добавить</button>
</template>
<style>

</style>