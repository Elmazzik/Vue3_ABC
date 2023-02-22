<script>
export default {
  data() {
    return {
      cat: ' ',
      tea: ' '
    }
  }
}
</script>
<template>
  <input class="text-field__input" v-model="cat">
  <p>{{ cat }}</p>
  <br>
  <a href="#" class="inline-link-1" >cat</a>
  <p ></p>
</template>
<style>

</style>