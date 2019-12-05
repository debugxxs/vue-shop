<template>
  <div class="login-box">
    <!-- 设置登录框 -->
    <div class="loginform-box">
      <!-- 登陆边框 -->
      <el-form ref="loginFromRef" :model="LoginForm" label-width="0px" class="loginformStyle">
        <!-- 用户表单 -->
        <el-form-item>
          <el-input placeholder="用户名" prefix-icon="el-icon-user"></el-input>
        </el-form-item>
        <!-- 密码表单 -->
        <el-form-item>
          <el-input placeholder="密码" prefix-icon="el-icon-key"></el-input>
        </el-form-item>
        <!-- 登陆按钮 -->
        <el-form-item class="btns">
          <el-button type="success" size="medium">登陆</el-button>
        </el-form-item>
      </el-form>
    </div>
  </div>
</template>
<script>
export default {
  name: 'login'
}
</script>
<style lang="less" scoped>
.login-box {
  width: 100%;
  height: 40%;
  background: #ffffff;
  display: flex;
  position: absolute;
  top: 35%;
}
.loginform-box {
  width: 350px;
  height: 95%;
  border: 1px solid #eee;
  border-radius: 20px;
  position: absolute;
  top: 5px;
  left: 65%;
  background-color: #ffffff80;
}
.loginform-box .loginformStyle {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 0 20px;
  box-sizing: border-box;
}
.btns {
  display: flex;
  justify-content: flex-end;
}
</style>
