<template>
  <tab-bar>
      <tab-bar-item path="/home"  >
         <img slot="item-icon" src="~assets/img/tabbar/home.svg">
         <img slot="item-icon-active" src="~assets/img/tabbar/home_active.svg">
      <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category">
          <img slot="item-icon" src="~assets/img/tabbar/category.svg">
          <img slot="item-icon-active" src="~assets/img/tabbar/category_active.svg">
      <div slot="item-text">分类</div>
      </tab-bar-item >
      <tab-bar-item path="/cart">
          <img slot="item-icon" src="~assets/img/tabbar/shopcart.svg">
          <img slot="item-icon-active" src="~assets/img/tabbar/shopcart_active.svg">
      <div slot="item-text">购物车</div>
      </tab-bar-item >
      <tab-bar-item path="/profile">
          <img slot="item-icon" src="~assets/img/tabbar/profile.svg">
          <img slot="item-icon-active" src="~assets/img/tabbar/profile_active.svg">
      <div slot="item-text">我的</div>
      </tab-bar-item>

    </tab-bar>
</template>

<script>
// 这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
import TabBar from '@/components/common/tabbar/TabBar'
import TabBarItem from '@/components/common/tabbar/TabBaritem'
export default {
  components: {
    TabBar,
    TabBarItem
  },
  // 定义属性
  data() {
    return {

    }
  },
  // 计算属性，会监听依赖属性值随之变化
  computed: {
  },
  // 监控data中的数据变化
  watch: {},
  // 方法集合
  methods: {

  },
  // 生命周期 - 创建完成（可以访问当前this实例）
  created() {

  },
  // 生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {

  },
  beforeCreate() {}, // 生命周期 - 创建之前
  beforeMount() {}, // 生命周期 - 挂载之前
  beforeUpdate() {}, // 生命周期 - 更新之前
  updated() {}, // 生命周期 - 更新之后
  beforeDestroy() {}, // 生命周期 - 销毁之前
  destroyed() {}, // 生命周期 - 销毁完成
  activated() {}, // 如果页面有keep-alive缓存功能，这个函数会触发
}
</script>

<style scoped>

</style>
