<template>
<div id='site-nav'>
  <nav>
    <div>
      <span><i class="icon iconfont icon-shouye"></i><a href="">天猫首页</a></span>
      <span><em>喵,欢迎来天猫</em><a href="">请登录</a><a href="">免费注册</a></span>
    </div>
    <div>
      <ul>
        <li><a href="">我的淘宝<b></b></a></li>
        <li><i class='icon iconfont icon-gouwuche3'></i><a href="">购物车</a></li>
        <li><a href="">收藏夹<b></b></a></li>
        <li></li>
        <li><i class='icon iconfont icon-shouji'></i><a href="">手机版</a></li>
        <li><a href="">淘宝网</a></li>
        <li><a href="">网页无障碍</a></li>
        <li><a href="">商家支持<b></b></a></li>
      </ul>
    </div>
  </nav>
</div>
</template>

<script>
export default {
  name: 'Navbar'

}
</script>

<style lang='scss' scoped>
#site-nav {
  height: 26px;
  line-height: 26px;
  font-size: 12px;
  color: #999;
  background-color: #f2f2f2;

  a {
    color: #999;
  }

  i {
    color: #ff0030;
  }

  nav {
    height: 100%;
    width: 990px;
    margin: auto;
  }
}

nav>div:first-child {
  float: left;
  >span:first-child {
    margin-right: 20px;
  }

  >span:last-child {
    >a {
      padding: 0 10px 0 20px;
    }
  }
}

nav>div:last-child {
  float: right;

  li {
    display: inline-block;
    padding: 0 10px;

    &:nth-child(4) {
      width: 0;
      height: 14px;
      border-left: 1px solid #ccc;
      margin-left: 12px;
      vertical-align: -2px;
    }

    &:nth-child(1), &:nth-child(3), &:nth-child(8) {
      position: relative;

      b {
        position: absolute;
        top: 12px;
        right: 1px;
        width: 0;
        height: 0;
        border-width: 3px;
        border-style: solid dashed dashed;
        border-color: #bbb transparent transparent;
      }
    }
  }
}



</style>