<template>
<div id='bottom'>
  <div>
    <a href=""></a><a href=""></a><a href=""></a><a href=""></a>
  </div>

  <div>
    <dl>
      <dt>购物指南</dt>
      <dd><a href="">免费注册</a><a href="">开通支付宝</a><a href="">支付宝充值</a></dd>
    </dl>
    <dl>
      <dt>天猫保障</dt>
      <dd><a href="">发票保障</a><a href="">售后规则</a><a href="">物流时效保障</a></dd>
    </dl>
    <dl>
      <dt>支付方式</dt>
      <dd><a href="">快捷支付</a><a href="">信用卡</a><a href="">余额宝</a><a href="">蚂蚁花呗</a>
      <a href="">货到付款</a></dd>
    </dl>
    <dl>
      <dt>商家服务</dt>
      <dd><a href="">天猫规则</a><a href="">商家入驻</a><a href="">商家中心</a><a href="">天猫必修课</a>
      <a href="">喵言喵语</a><a href="">运营服务</a></dd>
    </dl>
    <dl>
      <dt>手机天猫</dt>
      <dd><a href=""><img src="../../assets/img/TB14MWoNhjaK1RjSZFAwu2dLFXa.png" alt="" width="105" height="105"></a></dd>
    </dl>
  </div>
</div>
</template>

<script>
export default {
  name: 'Bottom'

}
</script>

<style lang="scss" scoped>
#bottom {
  background-color: rgb(240, 240, 240);
  overflow: hidden;

  >div:first-child {
    width: 1190px;
    height: 100px;
    margin: 25px auto;

    background: url('../../assets/img/TB14dANRXXXXXbdXXXXXXXXXXXX-1190-100.jpg') no-repeat;

    a {
      display: inline-block;
      width: 297px;
      height: 100px;
    }
  }

  >div:last-child {
    width: 1190px;
    height: 190px;
    padding-top: 22px;
    margin: auto;

    border-top: 1px solid #ededed;
    background: url('../../assets/img/下载.jpg') no-repeat 45px bottom;

    dl {
      float: left;
      width: 186px;
      padding-left: 52px;
    }

    dt {
      color: #646466;
      font-size: 16px;
      font-weight: 700;
      line-height: 30px;
    }

    dd a {
      display: block;
      color: #8b8b88;
      font-size: 12px;
      line-height: 20px;
    }

  }
}



</style>