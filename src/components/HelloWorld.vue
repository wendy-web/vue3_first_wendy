<template>
  <div class="hello">
    hello {{msg}}
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  beforeCreate() {

  },
  // 组件间的通信
  emits: ['sayHello'],
  setup(props, { emit }) {
    emit('sayHello', '2020')
  }
}
</script>
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
