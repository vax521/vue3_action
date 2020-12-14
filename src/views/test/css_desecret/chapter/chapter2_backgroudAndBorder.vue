<template>
  <div>
    <h2>2-6复杂背景图案</h2>
    <div class="complex-backgroud">hekko</div>
    <h2>2-8连续的图像边框</h2>
    <div class="image-border">
      <div>I have a nice stone image border,dont I look pretty?</div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'chapter2_backgroudAndBorder',
  }
</script>

<style scoped>
  .complex-backgroud {
    display: block;
    width: 200px;
    height: 200px;
    background: #58a linear-gradient(white 1px, transparent 0),
      linear-gradient(90deg, white 1px, transparent 0);
    background-size: 30px 30px;
  }
  .image-border {
    padding: 1em;
    background: linear-gradient(white, white), url('../static/button.png');
    background-clip: padding-box, border-box;
    background-origin: border-box;
    background-size: cover;
    border: 1px solid transparent;
  }
  .image-border > div {
    padding: 1em;
    background: white;
  }
</style>
