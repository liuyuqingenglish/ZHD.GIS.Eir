<template>
  <el-container>
    <el-header>标题栏
    </el-header>
  <el-container>
    <el-aside>侧边栏
      <router-view name="side"></router-view>
    </el-aside>
    <el-main>显示栏
      <router-view name="main">

      </router-view>
    </el-main>
  </el-container>
  </el-container>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  methods: {
    goto: function () {
      this.$router.push({ name: 'About' })
    }

  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
