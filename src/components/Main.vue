<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ subMsg }}</h2>
    <a href="#/list"><img src="../assets/main.jpg"></a>
    
  </div>
</template>

<script>
export default {
  name: 'Main',
  data () {
    return {
      msg: '치킨 구인/구직 사이트에 오신 것을 환영합니다.',
      subMsg: '(아래 이미지를 클릭해주세요)'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
h2 {
  color: #999;
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
