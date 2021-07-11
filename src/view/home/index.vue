<template>
  <div class="home">
    <van-row class="headBg">
      <van-nav-bar title="Home">
        <template #right>
          <svg class="menu-icon" aria-hidden="true">
            <use xlink:href="#icon-service"></use>
          </svg>
        </template>
      </van-nav-bar>
    </van-row>
    <van-tabbar v-model="active">
      <van-tabbar-item icon="wap-home-o">Home</van-tabbar-item>
      <van-tabbar-item icon="coupon-o">Rental</van-tabbar-item>
      <van-tabbar-item icon="friends-o">Team</van-tabbar-item>
      <van-tabbar-item icon="ellipsis">About</van-tabbar-item>
      <van-tabbar-item icon="manager-o">Me</van-tabbar-item>
    </van-tabbar>
  </div>
</template>

<script>

export default {
  data () {
    return {
       active: 0
    }
  }
};
</script>

<style lang="less" scoped>
.menu-icon {
  height: 24px;
  width: 24px;
  fill: white;
}
.headBg {
  position: relative;
    z-index: 1;
    min-height: 300px;
    padding-bottom: 60px;
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    background: #fff;
    background: url(../../assets/images/bg_top.png) no-repeat top/100%,#0eae6c;
    overflow-x: hidden;
}
.van-nav-bar {
  background: none;
  border: none;
}
/deep/ .van-nav-bar__content {
    height: 70px;
    line-height: 70px;
    & .van-nav-bar__title {
      color:white;
    }
}
.van-hairline--bottom{
  &::after {
    border: none;
  }
}
</style>
