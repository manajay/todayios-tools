<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      这里会收集一些平时常用的工具
      <a href="https://tool.lu/" target="_blank" rel="noopener">tools</a>.
    </p>
    <h3>短链接生成</h3>
    <ul>
      <li><a href="https://dwz.cn/" target="_blank" rel="noopener">百度短链接</a></li>
    </ul>
    <h3>图床</h3>
    <ul>
      <li><a href="https://sm.ms/" target="_blank" rel="noopener">sm.ms</a></li>
    </ul>
    <h3>代码美观</h3>
    <ul>
      <li><a href="https://carbon.now.sh/" target="_blank" rel="noopener">carbon</a></li>
    </ul>
    <h3>颜色单位转换</h3>
    <ul>
      <li><a href="https://www.color-hex.com/" target="_blank" rel="noopener">color-hex</a></li>
    </ul>
    <h3> json 格式化</h3>
    <ul>
      <li><a href="https://jsonformatter.curiousconcept.com/" target="_blank" rel="noopener">json-format</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
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
