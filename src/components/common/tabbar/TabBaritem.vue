<template>
  <div class="tab-bar-item" @click="itemClick">
    <!-- <div>首页</div> -->
    <div v-if="!isActive" ><slot  name="item-icon"></slot></div>
    <div v-else><slot  name="item-icon-active"></slot></div>
    <div :style="activeStyle"><slot name="item-text"></slot></div>
    </div>
</template>

<script>
export default {
  name: 'TabBarItem',
props:{
 path:String,
 activeColor:{
 type:String,
 default:'red'
 }
},
  data(){
       return{
        //  isActive:true
       }
  },
  computed:{
      isActive(){
        //判断当前活跃的路径和页面的路径
        // return this.$route.path.indexOf(this.path)!==-1
      },
      activeStyle(){
        //判断当前哪个活跃 哪个活跃用哪个颜色
        // return this.isActive ? {color:this.activeColor } : {}
      }
  },
  methods:{
    itemClick(){
      this.$router.replace(this.path)


    }
  },
  components:{

  }
}
</script>
<style scoped>
body{
  padding:0;
  margin:0
}
#tab-bar{
  display: flex;
  background-color: #f6f6f6;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  box-shadow: 0 -1px 1px rgba(100, 100, 100, .2)


}
.tab-bar-item {
  flex: 1;
   text-align:center;
  height: 49px;
  font-size :14px;
}
.tab-bar-item img {
  width:24px;
  height:24px;
  margin-top:3px;
  vertical-align:middle;
}
.active{
  color: palevioletred
}
</style>
