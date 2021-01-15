<template>
  <div>
    <h2>结构与布局</h2>
    <div>状态平滑的动画</div>
    <div class="panoramic"></div>
    <div>环形路径平移</div>
    <div class="path">
      <img src="http://lea.verou.me/book/adamcatlace.jpg" class="avatar" />
    </div>
  </div>
</template>
<script>
  export default {
    name: 'chapter7_buju',
  }
</script>

<style scoped>
  @keyframes panoramic {
    to {
      background-position: 100% 0;
    }
  }

  .panoramic {
    width: 150px;
    height: 150px;
    background: url('http://c3.staticflickr.com/3/2671/3904743709_74bc76d5ac_b.jpg');
    background-size: auto 100%;
    animation: panoramic 5s linear infinite alternate;
    animation-play-state: paused;
  }

  .panoramic:hover,
  .panoramic:focus {
    animation-play-state: running;
  }

  @keyframes spin {
    from {
      transform: rotate(0turn) translateY(-150px) translateY(50%) rotate(1turn);
    }
    to {
      transform: rotate(1turn) translateY(-150px) translateY(50%) rotate(0turn);
    }
  }

  .avatar {
    animation: spin 3s infinite linear;
  }

  /* Anything below this is just styling */

  .avatar {
    display: block;
    width: 50px;
    margin: calc(50% - 25px) auto 0;
    border-radius: 50%;
    overflow: hidden;
  }

  .path {
    width: 300px;
    height: 300px;
    padding: 20px;
    margin: 100px auto;
    border-radius: 50%;
    background: #fb3;
  }
</style>
