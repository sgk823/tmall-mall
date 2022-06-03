<template>
  <main>
    <div>
      <a href=""
        ><img
          src="../assets/img/TB1_Gn8RXXXXXXqaFXXXXXXXXXX-380-54.png"
          alt=""
          width="190"
      /></a>
    </div>
    <div>
      <div>
        <img
          src="../assets/img/TB1kcCBSpXXXXarapXXXXXXXXXX-1190-600.png"
          alt=""
        />
      </div>
      <form action="">
        <div><a href="">密码登录</a><a href="">短信登录</a></div>
        <div>
          <div><i class="el-icon-mobile-phone"></i></div>
          <el-input placeholder="请输入内容" v-model="input4">
            <el-select v-model="select" slot="prepend" placeholder="请选择">
              <el-option label="餐厅名" value="1"></el-option>
              <el-option label="订单号" value="2"></el-option>
              <el-option label="用户电话" value="3"></el-option>
            </el-select>
          </el-input>
        </div>
        <div>
          <div><i class="el-icon-receiving"></i></div>
          <el-input placeholder="请输入内容" v-model="input4">
        
          </el-input>
        </div>
        <div><el-button>登录</el-button></div>
        <div><a href="">免费注册</a></div>
      </form>
    </div>
    <div></div>
  </main>
</template>

<script>
export default {
  name: "Login",
};
</script>

<style lang="scss" scoped>
main > div:nth-child(1) {
  width: 1190px;
  margin: 0 auto;
  padding: 22px 0;
}

main > :nth-child(2) {
  position: relative;
  margin-bottom: 40px;
  background-color: rgb(181 2 1);

  > div {
    width: 1190px;
    height: 600px;
    margin: 0 auto;
  }

  form {
    position: absolute;
    top: 91px;
    right: 416px;

    background-color: #fff;
    width: 350px;
    min-height: 350px;
    padding: 25px 25px 45px;
  }
}
</style>