<template>
  <div id="app">
    <router-view></router-view>
    <TabBar>
      <TabBarItem path="/home">
        <div slot="icon" class="fa fa-home item-icon"></div>
        <div slot="text">首页</div>
      </TabBarItem>
      <TabBarItem path="/category">
        <div slot="icon" class="fa fa-th-large item-icon"></div>
        <div slot="text">分类</div>
      </TabBarItem>
      <TabBarItem path="/cart">
        <div slot="icon" class="fa fa-shopping-cart item-icon"></div>
        <div slot="text">购物车</div>
      </TabBarItem>
      <TabBarItem path="/profile">
        <div slot="icon" class="fa fa-user item-icon"></div>
        <div slot="text">我的</div>
      </TabBarItem>

    </TabBar>
  </div>
</template>

<script>
  import TabBar from "./components/common/tabbar/TabBar"
  import TabBarItem from "./components/common/tabbar/TabBarItem"
export default {
  name: 'App',
  components: {
    TabBar,
    TabBarItem
  }
}
</script>

<style>
  @import "./assets/css/font-awesome-4.7.0/css/font-awesome.min.css";
  @import "./assets/css/base.css";
.item-icon{
    font-size: 26px;
  }



</style>
