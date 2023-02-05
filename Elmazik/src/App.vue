<script>
export default {
  data() {
    return {
      str: "string",
    };
  },
  methods: {
    show: function () {
      let text = this.cape(this.text);
      alert(text);
    },
    cape: function (str) {
      return str[0].toUpperCase() + str.slice(1);
    },
  },
};
</script>

<template>
  <div>
    <button @click="show()">Тык!</button>
  </div>
</template>
