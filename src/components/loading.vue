<template>
  <div id="c-loading">
    <div :class="animationName"></div>
  </div>
</template>
<script>

export default {
  name: 'loading',
  props: {
    animationName: String,
    width: Number,
    height: Number
  },
  data() {
    return {
    }
  }
}

</script>
<style>

</style>

