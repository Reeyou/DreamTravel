<template>
  <div class="login">
    <div class="title">
      <h2>欢迎登陆</h2>
    </div>
    <div class="container">
      <form action="">
        <div>
          <i></i>
          <input type="text" placeholder="请输入用户名">
        </div>
        <p class='err_msg'></p>
        <div>
          <i></i>
          <input type="password" placeholder='请输入密码'>
        </div>
        <p class='err_msg'></p>
         
      </form>
      <button type='button'>登录</button>
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
        <span class='last'>没有账号？<a href="/#/register">前往注册</a></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Login', // 登录
  data() {
    return {

    }
  },
}
</script>

<style>

</style>
