<template>
  <div>
    <div class="extra">
      <span class="count">月售{{food.sellCount}}份</span><span>好评率{{food.rating}}%</span>
    </div>
    <div class="price">
      <span class="now">￥{{food.price}}</span><span class="old" v-show="food.oldPrice">￥{{food.oldPrice}}</span>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    food: {
      type: Object
    }
  }
};
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .extra
    line-height: 10px
    font-size: 10px
    color: rgb(147, 153, 159)
    margin-bottom: 6px
    .count
      margin-right: 12px
  .price
    font-weight: 700
    line-height: 24px
    .now
      margin-right: 8px
      font-size: 14px
      color: rgb(240, 20, 20)
    .old
      text-decoration: line-through
      font-size: 10px
      color: rgb(147, 153, 159)
</style>



