<script>
export default {
  data() {
  return {
    cssClasses: 'active valid',
  }
  }
}
</script>
<template>
<p :class="cssClasses">text</p>
</template>
<style>
p {
  	  color:darkslateblue;
      background-color: rgb(211, 214, 219);
  	}
</style>