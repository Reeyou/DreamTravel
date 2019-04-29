<template>
    <div class="resetPwd">
    <div class="title">
      <h2>忘记密码</h2>
    </div>
    <div class="container">
      <div class='getVCode'>
        <form action="">
          <div>
            <i></i>
            <input type="text" placeholder="请输入手机号">
          </div>
          <p class='err_msg'></p>
          <div>
            <i></i>
            <input type="password" placeholder='请输入验证码'>
            <p>获取验证码</p>
          </div>
          <p class='err_msg'></p>
          
        </form>
        <button type='button'>确认找回</button>
      </div>
      <div class='resetPassword'>
        <form action="">
          <div>
            <i></i>
            <input type="text" placeholder="请输入密码">
          </div>
          <p class='err_msg'></p>
          <div>
            <i></i>
            <input type="password" placeholder='请确认密码'>
          </div>
          <p class='err_msg'></p>
          
        </form>
        <button type='button'>修改密码</button>
      </div>
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
