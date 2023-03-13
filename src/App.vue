<template>
  <HelloWorld v-if="width > 1000" msg="Welcome to Your Vue.js App" />
  <MobileHome v-else />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MobileHome from './components/MobileHome.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    MobileHome
  },
  data () {
    return {
      width: window.innerWidth
    }
  },
  mounted () {
    window.onresize = ((wx) => {
      this.width = wx.currentTarget.innerWidth
      // console.log(this.width);
    })
    console.log(this.width);
  }
}
</script>

<style>
body {
  margin: 0px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
