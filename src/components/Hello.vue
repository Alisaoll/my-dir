<template>
  <div id="adver">
   <img :src="tab1" alt="">
  </div>

 <div id="search">
  <input type="text" class="search" placeholder="请输入旅游景点或城市">
  <button class="button">搜索</button>
</div>
</template>

<script>
var tab1= require('../assets/adver.png');
export default {
  data () {
    return {
      tab1:tab1,
      msg: 'Hello World!'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
