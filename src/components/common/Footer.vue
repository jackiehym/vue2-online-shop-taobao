<template>
<div class="footer">
  <van-tabbar v-model="active" active-color="orange" inactive-color="#000">
    <van-tabbar-item to="/" name="home" icon="home-o">首页</van-tabbar-item>
    <van-tabbar-item to="/categories" name="cate" icon="apps-o">分类</van-tabbar-item>
    <van-tabbar-item to="messages" name="chat" icon="chat-o" badge="10">消息</van-tabbar-item>
    <van-tabbar-item to="cart" name="cart" icon="shopping-cart-o">购物车</van-tabbar-item>
    <van-tabbar-item to="user" name="user" icon="user-circle-o">我的淘宝</van-tabbar-item>
  </van-tabbar>
</div>
</template>

<script>
import {Tabbar, TabbarItem} from 'vant'

export default {
  name: "Footer",
  components: {
    [Tabbar.name]: Tabbar,
    [TabbarItem.name]: TabbarItem
  },
  data() {
    return {
      active: 'home'
    }
  }
}
</script>

<style lang="less" scoped>
</style>
