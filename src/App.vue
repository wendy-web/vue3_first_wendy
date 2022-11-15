<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App" @sayHello = sayHelloHandle />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  
  beforeCreate() {
    console.log('before create');
  },
  created () {
    console.log('create');
  },
  beforeMount() {
    console.log('before mount');
  },
  mounted: function() {
    console.log('mount');
    this.init();
  },
  beforeUpdate() {
    console.log('before update');
  },
  methods: {
    sayHelloHandle(data) {
      console.log("app", data)
    },
    init() {
      console.log('fef');
      console.log(process.env.VUE_APP_BASE_URL, '-----------');
      console.log(process.env.NODE_ENV, '-e----------');

    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
