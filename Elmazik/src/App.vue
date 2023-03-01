<script>
import Employee from './components/Employee.vue'
export default {
  components: {
    Employee
  },
  data() {
    return {
    }
  },
  methods: {
    one: function () {
      document.write('Котики')
    },
    two: function () {
      document.write('Собачки')
    }
  }
}
</script>


<template>
  <Employee @show1="one" @show2="two" />
</template>
<style>

</style>