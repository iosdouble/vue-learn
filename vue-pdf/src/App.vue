<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>
    <button type="button" class="btn btn-primary" v-on:click="getPdf()">导出PDF</button>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      htmlTitle: '页面导出PDF文件名'
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
