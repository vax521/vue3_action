<template>
  <div>
    <h2 class="chapter-title" @click="goToChapter2">2-背景与边框</h2>
    <h2 class="chapter-title" @click="goToChapter3">3-形状</h2>
  </div>
</template>

<script>
  export default {
    name: 'index',
    methods: {
      goToChapter2() {
        this.$router.push('/test/chapter2')
      },
      goToChapter3() {
        this.$router.push('/test/chapter3')
      },
    },
  }
</script>

<style scoped>
  .chapter-title {
    margin-left: 20px;
    background-color: white;
  }
  .chapter-title:hover {
    cursor: pointer;
  }
</style>
