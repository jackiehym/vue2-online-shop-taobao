<template>
  <van-goods-action>
    <van-goods-action-icon icon="chat-o" text="客服" color="#ee0a24" />
    <van-goods-action-icon icon="cart-o" text="购物车" />
    <van-goods-action-icon icon="star" text="已收藏" color="#ff5000" />
    <van-goods-action-button type="warning" text="加入购物车" />
    <van-goods-action-button type="danger" text="立即购买" />
  </van-goods-action>
</template>

<script>
import { GoodsAction, GoodsActionIcon, GoodsActionButton } from 'vant'

export default {
  name: "GoodFooter",
  components: {
    [GoodsAction.name]: GoodsAction,
    [GoodsActionIcon.name]: GoodsActionIcon,
    [GoodsActionButton.name]: GoodsActionButton,
  }
}
</script>

<style scoped>

</style>
