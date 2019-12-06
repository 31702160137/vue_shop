<template>
  <div id="app">
    <img class="icon-logo" src="./assets/logo.png">
    <img class="icon-logo2" src="./assets/logo.png">
    <div>
      <p>
        If Element is successfully added to this project, you'll see an
        <code v-text="'<el-button>'"></code>
        below
      </p>
      <el-button>el-button</el-button>
    </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
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
.icon-logo{
  animation: rotes 1s ease-in-out alternate infinite;
}
.icon-logo2{
  animation: ss .1s ease-in-out alternate infinite;
}
@keyframes ss {
  from{
    transform: translateX(-10px);
  }
  to{
    transform: translateX(10px);
  }
}
@keyframes rotes {
  from{}
  to{
    transform: translateX(100px) rotate(180deg);
  }
}
@keyframes rotess {
  from{
    transform: scale(.5) rotate(180deg);
  }
  to{
    transform: scale(1) translateX(-100px) translateY(175px) rotate(360deg);
  }
}
</style>
