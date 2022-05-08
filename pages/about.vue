<template>
  <div>
    <h1>About</h1>
    <!-- a 标签会刷新导航，走服务端渲染 -->
    <h2>a标签</h2>
    <a href="/">首页</a>
    <!-- router-link组件 -->
    <h2>router-link</h2>
    <router-link to="/">首页</router-link>
    <!-- 编程式导航 -->
    <h2>编程式导航</h2>
    <button @click="onClick">按钮</button>
  </div>
</template>

<script>
export default {
  name: 'About',
  methods: {
    onClick () {
      this.$router.push('/')
      console.log('Hello')
    }
  }
}
</script>

<style>

</style>