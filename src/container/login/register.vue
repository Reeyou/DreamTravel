<template>
    <div class="register">
    <div class="title">
      <h2>欢迎注册</h2>
    </div>
    <div class="container">
      <form action="">
        <div>
          <i></i>
          <input type="text" placeholder="请输入手机号">
        </div>
        <p class='err_msg'></p>
        <div>
          <i></i>
          <input type="password" placeholder='请输入密码'>
        </div>
        <p class='err_msg'></p>
        <div>
          <i></i>
          <input type="password" placeholder='请确认密码'>
        </div>
        <p class='err_msg'></p>
        <div>
          <i></i>
          <input type="password" placeholder='请确认验证码'>
          <p>获取验证码</p>
        </div>
        <p class='err_msg'></p>
         
      </form>
      <button type='button'>注册</button>
      <div>
        <ul>
          <li>
            <div></div>
            <p>QQ登录</p>
          </li>
          <li>
            <div></div>
            <p>微信登录</p>
          </li>
        </ul>
      </div>
      <div class="tips">
        <span class='first'><a href="/#/resetPwd">忘记密码？</a></span>
        <span class='last'>已有账号？<a href="/#/register">马上登陆</a></span>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'Register', // 注册
  data() {
    return {

    }
  },
}
</script>

<style>

</style>
