<template>
  <div id="tour">
  <hgroup>
    <h2>热门旅游</h2>
    <h3>最新的各种热门旅游资讯的推荐！</h3>
  </hgroup>
  <div class="container">
    <figure v-for='items in itemss'>
      <img :src="pic" alt="">
      <figcaption>
        <h4>{{items.title}}</h4>
        <p>{{items.info}}</p>
        <div class="info">
          <em class="sat">满意度{{items.sat}} </em>
          <span class="price">¥ <strong>{{items.price}}</strong> 起</span>
        </div>
      </figcaption>
    </figure>
    
    <div class="clearfix"></div>
  </div>
</div>
</template>
<script>
var pic = require('../assets/tour1.png');
export default {
  data () {
    return {
     pic:pic,
     itemss:[
      {title:'曼谷-芭提雅6 日游',info:'包团特惠，超丰富景点',sat:'70%',price:2864},
      {title:'曼谷-芭提雅6 日游',info:'包团特惠，超丰富景点',sat:'70%',price:2864},
      {title:'曼谷-芭提雅6 日游',info:'包团特惠，超丰富景点',sat:'70%',price:2864},
      {title:'曼谷-芭提雅6 日游',info:'包团特惠，超丰富景点',sat:'70%',price:2864},]
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
