<script>
export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'name1',
          salary: 100,
          age: 30,
        },
        {
          id: 2,
          name: 'name2',
          salary: 200,
          age: 40,
        },
        {
          id: 3,
          name: 'name3',
          salary: 300,
          age: 50,
        },
      ],
    }
  },
  methods: {
    removeUser: function (id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;
      })
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
  <button @click="removecat">delete</button>
</template>
<style>

</style>