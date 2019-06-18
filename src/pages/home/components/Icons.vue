<template>
  <div class="icons">
    <div class="icon">icon1
      <!-- <img src="http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png"> -->
      <p>热门景点</p>
    </div>
<!--     <div class="icon">icon2</div>
<div class="icon">icon3</div>
<div class="icon">icon4</div>
<div class="icon">icon5</div>
<div class="icon">icon6</div>
<div class="icon">icon7</div>
<div class="icon">icon8</div> -->
  </div>
</template>

<script>
export default {
  name: 'HomeIcons'
}
</script>

<style lang="stylus" scoped>
  .icons
    overflow: hidden
    height: 0
    width: 100%
    padding-bottom: 50%
    background: green
    .icon
      float: left
      overflow: hidden
      height: 0
      width: 25%
      padding-bottom: 25%
      background: red
</style>
