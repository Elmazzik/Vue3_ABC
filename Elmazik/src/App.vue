<script>
export default {
  data() {
    return {
      isValid: true,
      isDisabled: true,
    }
  }
}
</script>
<template>
  <p :class="{ valid: isValid, disable: isDisabled }">котики!</p>
</template>
<style>

</style>