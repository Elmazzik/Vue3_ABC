<script>
export default {
  data() {
    return {
      day_week: 'Понедельник',
      num1: ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье'],
      day: '1',
      num2: ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14', '15', '16', '17', '18', '19', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', ' 31'],
      month: 'Январь',
      num3: ['Январь', 'Февраль', 'Март', 'Апрель', 'Май', 'Июнь', 'Июль', 'Август', 'Сентябрь', 'Октябрь', 'Ноябрь', 'Декабрь'],
      year: '2023',
      num4: ['2023', '2022', '2021', '2020', '2019', '2018']
    }
  }
}
</script>
<template>
      <select v-model="day_week">
      <option v-for="num1 in num1">{{ num1 }}</option>
      </select>
  <br>
  <select v-model="day">
  <option v-for="num2 in num2">{{ num2 }}</option>
  </select>
  <br>
  <select v-model="month">
  <option v-for="num3 in num3">{{ num3 }}</option>
  </select>
  <br>
  <select v-model="year">
  <option v-for="num4 in num4">{{ num4 }}</option>
  </select>
</template>
<style>

</style>