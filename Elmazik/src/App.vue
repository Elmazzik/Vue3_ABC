<script>
export default {
  data() {
	return {
		text: 'str',
	}
}
  methods: {
	show: function() {
		alert(this.text);
	}
}
};
</script>

<template>
  <button @click="show">text</button>
</template>
