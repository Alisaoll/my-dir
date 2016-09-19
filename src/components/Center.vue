<template>
    <tab1 v-if='tabs==0'></tab1>
    <tab2 v-if='tabs==1'></tab2>
    <tab3 v-if='tabs==2'></tab3>
    <tab4 v-if='tabs==3'></tab4>

</template>

<script>
import Tab1 from './Tab1'
import Tab2 from './Tab2'
import Tab3 from './Tab3'
import Tab4 from './Tab4'
export default {
 props: [
            'tabs'
        ],
  components: {
       Tab1,Tab2,Tab3,Tab4
    },
  data () {
     return{
     i:0
     }
  },


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>