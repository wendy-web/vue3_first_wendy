<!--
 * @Author: wendy-web wendywen@tencent.com
 * @Date: 2022-11-03 13:06:09
 * @LastEditors: wendy-web wendywen@tencent.com
 * @LastEditTime: 2022-11-03 13:06:36
 * @FilePath: /test_vue/src/components/child.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <div class="hello">
    child
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
