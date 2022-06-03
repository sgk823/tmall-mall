<template>
  <div class="container">
    <div>
      <ul>
        <li><i>1</i><span>设置用户名</span></li>
        <li><i>2</i><span>填写账号信息</span></li>
        <li><i>3</i><span>设置支付方式</span></li>
        <li><i>4</i><span>注册成功</span></li>
      </ul>
    </div>
    <div>
      <form action="">
        <div>
          <label for="">手机号码</label>
          <el-input
            placeholder="请输入您的手机号码"
            v-model="input3"
            class="input-with-select"
          >
            <el-select
              v-model="select"
              slot="prepend"
              placeholder="中国大陆  +86"
              style="width: 150px"
            >
              <el-option label="餐厅名" value="1"></el-option>
              <el-option label="订单号" value="2"></el-option>
              <el-option label="用户电话" value="3"></el-option>
            </el-select>
          </el-input>
        </div>
        <div></div>
        <p><el-button style="width:180px" disabled>下一步</el-button></p>
      </form>
    </div>
    <div v-show="showAgreement">
      <p><span>注册协议</span><span @click="showAgreement = false">✖</span></p>
      <p>
        <b>【审慎阅读】</b>您在申请注册流程中点击同意前,应当认真阅读以下协议。<b
          >请您务必审慎阅读、充分理解协议中相关条款内容,其中包括:</b
        >
      </p>
      <p>1、<b>与您约定免除或限制责任的条款:</b></p>
      <p>2、<b>与您约定法律适用和管辖的条款:</b></p>
      <p>3、<b>其他以粗体下划线标识的重要条款。</b></p>
      <p>如您对协议有任何疑问,可向平台客服咨询。</p>
      <p>
        <b>【特别提示】</b
        >当您按照注册页面提示填写信息、阅读并同意协议且完成全部注册程序后,即表示您已充分阅读、理解并接受协议的全部内容。
        如您因平台服务与淘宝发生争议的,适用《淘宝平台服务协议》处理。如您在使用平台服务过程中与其他用户发生争议的,依您与其他用户达成的协议处理。
      </p>
      <p>
        <b
          >阅读协议的过程中,如果您不同意相关协议或其中任何条款约定,您应立即停止注册程序</b
        >
      </p>
      <p><a href="">淘宝平台服务协议</a></p>
      <p><a href="">隐私权政策</a></p>
      <p><a href="">法律声明</a></p>
      <p><a href="">支付宝及客户端服务协议</a></p>
      <p><button>同意协议</button></p>
    </div>
    <div v-show="showHelp">
      <div><i @click="showHelp = false">✖</i></div>
      <div>
        <ul>
          <li>淘宝账户名是指什么?</li>
          <li>忘记会员名,怎么找回?</li>
          <li>忘记淘宝账号密码,怎么找回?</li>
          <li>手机(停机、丢失等)收不到验证码,怎么办?</li>
          <li>手机、邮箱正常使用,但是接收不到验证码,怎么办?</li>
        </ul>
        <p>
          <svg
            class="icon-talk"
            viewBox="0 0 38 38"
            style="width: 16px; height: 16px"
          >
            <path
              d="M13.8 31.2l1.1.3c1.3.3 2.7.5 4.1.5 8.9 0 16-6.5 16-14.5S27.9 3 19 3 3 9.5 3 17.5c0 3.6 1.5 7.1 4.1 9.7l.9.9v6.2zm.4 3.2L8 37.7c-.3.2-.7.3-1 .3-1.1 0-2-.9-2-2v-6.7C1.9 26.2 0 22 0 17.5 0 7.8 8.5 0 19 0s19 7.8 19 17.5S29.5 35 19 35c-1.7 0-3.3-.2-4.8-.6zm1.3-20.9c0-1.7 1.2-3 3.5-3 2.5 0 3.9 1.7 3.5 3.1-.3 1-.7 1.6-1.8 2.3-.1.1-.6.4-.5.3-1.9 1.3-2.8 2.5-2.8 4.7 0 .8.7 1.5 1.5 1.5s1.5-.7 1.5-1.5c0-1.1.3-1.5 1.5-2.3-.1.1.4-.2.5-.3 1.6-1.1 2.5-2.2 3-4.1.8-3.3-2-6.9-6.5-6.9-4.1 0-6.5 2.7-6.5 6 0 .8.7 1.5 1.5 1.5.9.2 1.6-.5 1.6-1.3zM19 28c1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2 .9 2 2 2z"
            ></path>
          </svg>
          <span>点我提问</span>
        </p>
      </div>
    </div>
    <div v-show="!showHelp">
      <p>
        <svg viewBox="0 0 140 140" xmlns="http://www.w3.org/2000/svg">
          <g fill="currentColor" fill-rule="evenodd">
            <path
              d="M95.008 119.346c16.45-8.633 27.647-25.384 27.647-43.042 0-5.822-.717-10.419-2.23-14.047-3.457-12.333-15.596-21.498-30.044-21.498-7.328 0-14.337 3.46-19.881 7.702-5.544-4.3-12.617-7.702-19.881-7.702-14.383 0-26.55 9.15-30.033 21.469-1.52 3.632-2.241 8.238-2.241 14.076 0 17.658 11.196 34.409 27.647 43.042-.6.868-1.025 1.94-1.275 3.142-.243 1.169-.332 2.501-.281 3.92C22.993 116.939 10 95.722 10 71.069 10 37.59 32.914 10.45 70.5 10.45S131 37.591 131 71.068c0 24.653-12.993 45.87-34.436 55.34.051-1.419-.038-2.751-.281-3.92-.25-1.202-.675-2.274-1.275-3.142z"
            ></path>
            <path
              d="M72.9 126.127s12.202-5.939 17.745-5.939c5.543 0 2.063 18.812-3.48 18.812-5.542 0-14.822-9.399-14.822-9.399-1.27-1.185-1.009-2.749.557-3.474zm-4.8 0c1.566.725 1.827 2.29.557 3.474 0 0-9.28 9.399-14.823 9.399-5.542 0-9.022-18.812-3.479-18.812s17.745 5.94 17.745 5.94zM44.422 72.87c0-2.15 2.014-3.893 4.502-3.893h.384c2.486 0 4.502 1.745 4.502 3.892v17.3c0 2.149-2.013 3.891-4.502 3.891h-.384c-2.486 0-4.502-1.744-4.502-3.892V72.87zm42.768 0c0-2.15 2.013-3.893 4.502-3.893h.384c2.486 0 4.502 1.745 4.502 3.892v17.3c0 2.149-2.014 3.891-4.502 3.891h-.384c-2.486 0-4.502-1.744-4.502-3.892V72.87zm27.642-53.013c3.825-3.115 5.737-6.594 5.737-10.436C120.569 3.657 118 0 114.832 0c-3.169 0-5.737 3.657-5.737 9.42 0 3.843 1.912 7.322 5.737 10.437zm-88.664 0c3.825-3.115 5.737-6.594 5.737-10.436C31.905 3.657 29.337 0 26.168 0 23 0 20.431 3.657 20.431 9.42c0 3.843 1.912 7.322 5.737 10.437z"
            ></path>
          </g>
        </svg>
      </p>
      <p>有问题?</p>
      <p>找小蜜</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Register",
  data() {
    return {
      showAgreement: true,
      showHelp: true,
      input3: ''
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  position: relative;
  width: 990px;
  margin: 0 auto;

  > div:first-child {
    height: 46px;
    border-bottom: 2px solid #e6e6e6;

    ul {
      width: 720px;
      height: 100%;
      margin: auto;

      display: flex;
      align-items: center;
      justify-content: space-between;

      li {
        width: 150px;
        line-height: 46px;
        padding-left: 30px;
        font-size: 16px;
        color: #999;
        font-weight: 700;

        i {
          display: inline-block;
          width: 24px;
          height: 24px;
          border-radius: 24px;
          background-color: #d8d8d8;
          font-size: 14px;
          line-height: 24px;
          margin-right: 5px;
          color: #fff;
          text-align: center;
        }

        &:first-child {
          border-bottom: 2px solid #ff4700;
        }

        &:first-child i {
          background-color: #f00;
        }

        &:first-child span {
          color: #3e3e3e;
        }
      }
    }
  }

  > div:nth-child(3) {
    position: absolute;
    top: 118px;
    left: 133px;

    width: 680px;
    padding: 20px;
    border: 2px solid #dedede;
    border-top-color: #ff4a00;

    font-size: 13px;
    line-height: 28px;

    b {
      font-weight: bold;
    }

    a {
      font-size: 14px;
      font-weight: 700;
      color: #ff0036;
    }

    > p:nth-child(1) {
      display: flex;
      justify-content: space-between;

      span:nth-child(1) {
        font-size: 16px;
        font-weight: bold;
        color: #3e3e3e;
      }

      span:nth-child(2) {
        font-size: 20px;
        color: #f00;
        cursor: pointer;
      }
    }

    > p:last-child {
      text-align: center;
      button {
        width: 180px;
        height: 36px;
        background-color: #ff0036;
        color: #fff;
        font-size: 16px;
        font-weight: 700;
        border: none;
        border-radius: 3px;
        cursor: pointer;

        &:hover {
          background-color: rgba(255, 0, 54, 0.8);
        }
      }
    }
  }

  > div:nth-child(4) {
    position: fixed;
    top: 300px;
    right: 22%;

    > div:first-child {
      position: relative;
      width: 60px;
      height: 82px;
      background-image: url("../assets/img/TB1yJ1Qw3HqK1RjSZFgXXa7JXXa-119-164.svg");
      background-size: contain;
      margin-left: 30px;

      i {
        position: absolute;
        top: 0;
        right: -25px;

        display: block;
        width: 16px;
        height: 16px;
        border-radius: 16px;
        background-color: #000;
        color: #fff;
        font-size: 10px;
        line-height: 16px;
        text-align: center;
        cursor: pointer;
      }
    }

    > div:last-child {
      border: 2px solid #ffb300;
      box-shadow: 0 10px 20px 0 rgb(0 0 0 / 30%);
      border-radius: 12px;
      font-size: 12px;
      width: 125px;
      line-height: 18px;

      ul {
        margin-top: 10px;

        li {
          padding: 5px;
        }
      }

      p {
        text-align: center;
        height: 23px;
        width: 100%;
        background-color: #f7931e;
        border-radius: 0 0 10px 10px;
        padding: 5px 0 3px 0;
        color: #fff;
        font-size: 15px;
        fill: currentColor;
      }
    }
  }

  > div:last-child {
    position: fixed;
    top: 300px;
    right: 22%;

    width: 68px;
    border: 2px solid #f5f5f5;
    color: #b7b7b7;
    border-radius: 4px;
    text-align: center;
    font-size: 14px;
    padding: 8px 0;
    line-height: 18px;

    &:hover {
      border-color: #f7931e;
      color: #f7931e;
      cursor: pointer;
    }

    svg {
      color: #f7931e;
      width: 32px;
      height: 32px;
    }
  }

  > div:nth-child(2) {
    padding: 50px 0;

    form {
      width: 720px;
      margin: 0 auto;
      padding: 10px 0;

      >div {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 120px 10px 120px;

        label {
          width: 96px;
        }
      }

      >p {
       text-align: center;
      }
    }
  }
}
</style>