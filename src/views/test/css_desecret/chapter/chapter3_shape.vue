<template>
  <div>
    <h2>3-1 border-radius</h2>
    <div class="self-adaption-circle">自适应圆形</div>
    <div class="tuoyuan"></div>
    <!--参考资料：https://simurai.com/archive/buttons/#-->
    <h2>sweet buttons</h2>
    <a href="#" class="button">Button</a>
    <a href="#" data-icon="✆" class="button blue brackets">Call</a>
    <a href=" " data-icon="✰" class="button pink skew glossy">Stars</a>
  </div>
</template>

<script>
  export default {
    name: 'chapter3_shape',
  }
</script>

<style scoped>
  .self-adaption-circle {
    width: 200px;
    height: 200px;
    background: #fb3;
    border-radius: 100px;
  }
  .tuoyuan {
    width: 300px;
    height: 200px;
    background: #fb3;
    border-radius: 50%/50%;
  }
  .button {
    position: relative;
    display: inline-block;
    padding: 0.5em 0.6em 0.4em 0.6em;
    margin: 0.5em;
    font: 24px sans-serif;
    font-weight: bold;
    color: hsl(0, 0%, 40%);
    background-color: hsl(0, 0%, 75%);
    text-decoration: none;
    background-image: -webkit-gradient(
        radial,
        50% 0,
        100,
        50% 0,
        0,
        from(rgba(255, 255, 255, 0)),
        to(rgba(255, 255, 255, 0.7))
      ),
      url('../static/noise.png');
    text-shadow: rgba(255, 255, 255, 0.5) 0 1px 0;
    /*控制用户能否选中文本*/
    user-select: none;
    border-top: 1px solid rgba(255, 255, 255, 0.8);
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    transition: background 0.2s ease-in-out;
    box-shadow: inset rgba(255, 254, 255, 0.6) 0 0.3em 0.3em,
      inset rgba(0, 0, 0, 0.15) 0 -0.1em 0.3em,
      /* inner shadow */ hsl(0, 0%, 60%) 0 0.1em 3px,
      hsl(0, 0%, 45%) 0 0.3em 1px,
      /* color border */ rgba(0, 0, 0, 0.2) 0 0.5em 5px;
  }
  .button:before {
    font: 1.2em/0 sans-serif;
    content: attr(data-icon);
    margin-right: 6px;
  }
  .button.blue {
    color: hsl(208, 50%, 40%);
    background-color: hsl(208, 100%, 75%);
    box-shadow: inset rgba(255, 254, 255, 0.6) 0 0.3em 0.3em,
      inset rgba(0, 0, 0, 0.15) 0 -0.1em 0.3em,
      /* inner shadow */ hsl(208, 50%, 55%) 0 0.1em 3px,
      hsl(208, 50%, 40%) 0 0.3em 1px,
      /* color border */ rgba(0, 0, 0, 0.2) 0 0.5em 5px;
  }
  .brackets,
  .brackets.glossy:after,
  .brackets.glass:after {
    border-top: none;
    border-radius: 0.5em / 1em;
  }
  .button.pink {
    color: hsl(340, 100%, 30%) !important;
    background-color: hsl(340, 100%, 75%);
    -webkit-box-shadow: inset rgba(255, 254, 255, 0.6) 0 0.3em 0.3em,
      inset rgba(0, 0, 0, 0.15) 0 -0.1em 0.3em,
      /* inner shadow */ hsl(340, 70%, 50%) 0 0.1em 3px,
      hsl(340, 80%, 40%) 0 0.3em 1px,
      /* color border */ rgba(0, 0, 0, 0.2) 0 0.5em 5px;
    -moz-box-shadow: inset rgba(255, 254, 255, 0.6) 0 0.3em 0.3em,
      inset rgba(0, 0, 0, 0.15) 0 -0.1em 0.3em,
      /* inner shadow */ hsl(340, 70%, 50%) 0 0.1em 3px,
      hsl(340, 80%, 40%) 0 0.3em 1px,
      /* color border */ rgba(0, 0, 0, 0.2) 0 0.5em 5px;
    box-shadow: inset rgba(255, 254, 255, 0.6) 0 0.3em 0.3em,
      inset rgba(0, 0, 0, 0.15) 0 -0.1em 0.3em,
      /* inner shadow */ hsl(340, 70%, 50%) 0 0.1em 3px,
      hsl(340, 80%, 40%) 0 0.3em 1px,
      /* color border */ rgba(0, 0, 0, 0.2) 0 0.5em 5px;
  }
  .skew {
    border-top: none;
    padding-right: 1.2em;
    padding-left: 0.8em;
    border-radius: 5em 1em / 5em 1em;
  }
</style>
