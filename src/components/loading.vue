<template>
  <div id="c-loading">
    <div :class="animation"></div>
  </div>
</template>
<script>

export default {
  name: 'loading',
  props: {
    animation: String,
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
.square {
  position: relative;
  box-sizing: border-box;
  width: 120px;
  height: 120px;
}

.suqare::before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  border-top: 2px solid #F07883;
  border-right: 2px solid #F07883;
}

.square::after {
  content: '';
  position: absolute;
  right: 0;
  bottom: 0;
  width: 100%;
  border-left: 2px solid #F07883;
  border-bottom: 2px solid #F07883;
}
</style>

