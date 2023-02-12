<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      obj: {
        user1: '100$',
        user2: '200$',
        user3: '300$',
      },
    }
  },
}
</script>

<template>
Задание №1
    <ul>
      <li v-for="elem in obj">
		{{ elem }}</li>
    </ul>
Задание №2
    <ul>
      <li v-for="(elem, key) in obj">
		{{ key }} {{ elem }}</li>
    </ul>
Задание №3
    <ul>
      <li v-for="(elem, key, index) in obj">
		{{ index }}
		{{ key }}
		{{ elem }}</li>
    </ul>
</template>
