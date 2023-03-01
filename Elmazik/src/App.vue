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
    },
    edit(user) {
      user.isEdit = true;
    },
    save(user) {
      user.isEdit = false;
    },
  }
}
</script>

<template>
  <table class="tb">
    <tr v-for="user in users" :key="user.id">
      <template v-if="!user.isEdit">
        <td class="block">{{ user.name }}</td>
        <td class="block">{{ user.salary }}</td>
        <td class="block">{{ user.age }}</td>
        <td class="block"><button class="btn" @click="removeUser(user.id)">delete</button></td>
        <td class="block"><button class="btn" @click="edit(user)">update</button></td>
      </template>
      <template v-else>
        <td class="block"><input class="block_input" v-model="user.name"></td>
        <td class="block"><input class="block_input" v-model="user.salary"></td>
        <td class="block"><input class="block_input" v-model="user.age"></td>
        <td class="block"><button class="btn" @click="save(user)">save</button></td>
      </template>
    </tr>
  </table>
</template>
<style>

</style>