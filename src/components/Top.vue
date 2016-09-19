<template>

   <header id="header">
    <nav class="link">
      <h2 class="none">网站导航</h2>
      <ul>
        <li v-for='item in items  'v-bind:class="{ 'active': item.activs}" :data='$index' v-on:click='greet(item,$index)'>{{item.title}}     
        </li>
      </ul>
    </nav>
</header>

</template>

<script>
export default {
 props: [
            'tabs'
        ],
  data () {
    return {
      items:[
      {title:'首页',activs:true},
      {title:'资讯',activs:false},
      {title:'票务',activs:false},
      {title:'关于',activs:false}]
    }

  },
   methods: {
    greet: function (item,index) {
           this.tabs=index;
          for(var i=0;i<this.items.length;i++){
               if(index==i){
                  if(item.activs==false){
                    item.activs=!item.activs;
                  }
                
                }else{
                this.items[i].activs=false;
                }
          }
     
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
