<template>
<footer>
  <div>
    <div class='container'>
      <div>
        <a href="">关于天猫</a><a href="">商家服务大厅</a><a href="">开放平台</a><a href="">诚聘英才</a>
        <a href="">联系我们</a><a href="">网站合作</a><a href="">法律声明</a><a href="">隐私权政策</a>
        <a href="">知识产权</a><a href="">廉政举报</a><a href="">不正当竞争举报</a>
      </div>
      <div>
        <a href="">阿里巴巴集团</a><span>|</span><a href="">淘宝网</a><span>|</span><a href="">天猫</a><span>|</span>
        <a href="">聚划算</a><span>|</span><a href="">全球速卖通</a><span>|</span><a href="">阿里巴巴国际交易市场</a><span>|</span>
        <a href="">1688</a><span>|</span><a href="">阿里妈妈</a><span>|</span><a href="">飞猪</a><span>|</span>
        <a href="">阿里云计算</a><span>|</span><a href="">AliOS</a><span>|</span><a href="">阿里通信</a><span>|</span>
        <a href="">万网</a><span>|</span><a href="">高德</a><span>|</span><a href="">UC</a><span>|</span>
        <a href="">友盟</a><span>|</span><a href="">虾米</a><span>|</span><a href="">钉钉</a><span>|</span>
        <a href="">支付宝</a><span>|</span><a href="">阿里安全</a>
      </div>

      <div>
        <p><a href="">增值电信业务经营许可证:浙B2-20110446</a>
        <span>市场名称登记证: 工商网市字3301004119号</span><span>出版物网络交易平台服务经营备案证: 新出发浙备字第2019002号</span></p>
        <p>
          <span>互联网违法和不良信息举报电话: 0571-81683755 blxxjb@alibaba-inc.com</span>
          <span>互联网药品信息服务资质证书编号: </span>
          <a href="">浙-(经营性)-2017-0005</a><a href=""><img src="../../assets/img/TB1yEqRP.png" alt="">浙公网安备 33010002000120号</a>
        </p>
        <p><span>医疗器械网络交易服务第三方平台备案:(浙)网械平台备字[2018]第00002号</span></p>
        <p>
          <span>浙江省网络食品销售第三方平台提供者备案:浙网食A33010002</span>&nbsp;
          <a href="">12318举报</a>&nbsp;<a href="">浙B2-20110446-1</a>
        </p>
        <p><b>&copy;2003-现在 TMALL.COM 版权所有</b></p>
      </div>
    </div>

    <div><img src="../../assets/img/O1CN01Hs1MVu1IDvM07YrGh.png" alt="" width="146" height="71"></div>
  </div>

  <div></div>
</footer>
</template>

<script>
export default {
  name: 'Footer'

}
</script>

<style lang='scss' scoped>
footer {
  background-color: #000;

  >div:first-child {
    border-top: 2px solid #FF0036;

    >div:last-child {
      width: 146px;
      height: 71px;
      margin: 5px auto 0 680px;
      background-color: #fff;
    }

  }

  >div:last-child {
    height: 18px;
    background-color: #000;
  }
}

.container {
  width: 1190px;
  margin: auto;
  font-size: 12px;

  a {
    color: #fff;
    margin-right: 5px;

    &:hover {
      text-decoration: underline;
    }
  }

  >div:nth-child(1) {
    line-height: 25px;
    padding: 5px 0;
  }

  >div:nth-child(2){
    line-height: 25px;
    color: #fff;
    padding: 5px 0;

    a {
      margin-left: 5px;

      &:first-child {
        margin-left: 0;
      }
    }

  }

  >div:nth-child(3) {
    line-height: 20px;
    color: #a4a4a4;
    a {
      color: #a4a4a4;
    }

    >p:last-child {
      color: #686866;
    }
  }
}





</style>