<script>
import Employee from './components/Employee.vue'
export default {
  components: {
    Employee
  },
  data() {
    return {
      name: '"Эльмаз"',
      surn: 'Мустафаева',
      age: 18,
      value: true,
    }
  }
}
</script>

<template>
  <Employee :name="name" :surn="surn" :age="age" :value="value" />
</template>

<style>

</style>