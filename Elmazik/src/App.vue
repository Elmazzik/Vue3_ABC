<script>
import { normalizeProps } from 'vue';

export default {
  data() {
    return {
      items: [1, 2, 3],
      }
  },
}
</script>

<template>
  <div>
    <p>1</p>
    <p class="divider"></p>
  </div>
  <div>
    <p>2</p>
    <p class="divider"></p>
  </div>
  <div>
    <p>3</p>
    <p class="divider"></p>
  </div>
  <ul>
    <li>1</li>
    <li class="divider"></li>
    <li>2</li>
    <li class="divider"></li>
    <li>3</li>
    <li class="divider"></li>
  </ul>
</template>
