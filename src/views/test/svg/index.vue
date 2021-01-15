<template>
  <div>
    <h1>My first SVG</h1>

    <svg xmlns="http://www.w3.org/2000/svg" version="1.1">
      <circle
        cx="100"
        cy="50"
        r="40"
        stroke="black"
        stroke-width="2"
        fill="red"
      />
    </svg>
    <svg
      width="9px"
      height="15px"
      viewBox="0 0 9 15"
      version="1.1"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink"
    >
      <!-- Generator: Sketch 56 (81588) - https://sketch.com -->
      <title>前往icon</title>
      <desc>Created with Sketch.</desc>
      <g
        id="页面-1"
        stroke="none"
        stroke-width="1"
        fill="none"
        fill-rule="evenodd"
      >
        <g
          id="iPhone-XS"
          transform="translate(-331.000000, -319.000000)"
          fill="#FFFFFF"
        >
          <g id="内推职位" transform="translate(15.000000, 292.000000)">
            <g
              id="前往icon_白"
              transform="translate(315.769531, 34.500000) rotate(45.000000) translate(-315.769531, -34.500000) translate(309.269531, 28.000000)"
            >
              <rect id="矩形" x="2" y="0" width="11" height="2" rx="1"></rect>
              <rect
                id="矩形"
                transform="translate(12.000000, 5.500000) rotate(90.000000) translate(-12.000000, -5.500000) "
                x="6.5"
                y="4.5"
                width="11"
                height="2"
                rx="1"
              ></rect>
            </g>
          </g>
        </g>
      </g>
    </svg>
    <svg xmlns="http://www.w3.org/2000/svg" version="1.1">
      <rect
        x="50"
        y="20"
        width="150"
        height="150"
        style="fill: blue; stroke: pink; stroke-width: 5; opacity: 0.5"
      />
    </svg>
    <embed src="./data/circle.svg" type="image/svg+xml" />
    <a href="./data/circle.svg">查看 SVG 文件</a>
    <div>SVG动画</div>
    <div>
      <svg width="70" height="70" viewbox="0 0 70 70">
        <circle fill="black" cx="45" cy="45" r="25" />
      </svg>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'index',
  }
</script>

<style scoped></style>
