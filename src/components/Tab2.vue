<template>
  <div class="list information">
  <h2>热门旅游</h2>
  <figure v-for='item in itemss'>
    <img :src="tab" alt="">
    <figcaption>
      <hgroup>
        <h2 class="title">{{item.title}}</h2>
        <h3 class="small_title">{{item.info}}</h3>
      </hgroup>
      <div class="price">¥<strong>{{item.price}}</strong></div>
    </figcaption>
  </figure>
</div>
</template>

<script>
var tab= require('../assets/tour1.png');
export default {
  data () {
    return {
    tab:tab,
     itemss:[
      {title:'曼谷-芭提雅6 日游',info:'包团特惠，超丰富景点，升级1 晚国五，无自费，赠送600 元',price:2864,src:'../assets/adver.png'},
      {title:'马尔代夫6日自助游',info:'双鱼岛Olhuveli4晚，上海出发，机+酒 包含:早晚餐+快艇...',price:8039,src:'../assets/adver.png'},
      {title:'巴厘岛6日半自助游',info:'蓝梦出海，独栋别墅，悦榕庄下午茶，纯玩...',price:2864,src:'../assets/adver.png'},
      {title:'塞舌尔迪拜9日自助游',info:'一游两国，4晚塞舌尔，2晚迪拜，香港EK往返...',price:2864,src:'../assets/adver.png'},]
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
