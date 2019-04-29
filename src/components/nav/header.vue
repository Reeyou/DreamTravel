<template>
  <div class='navHead'>
    <div class='navHead_container'>
      <div class="logo">
        <img src="../../assets/logo-black.png" alt="">
      </div>
      <div class="nav">
        <ul>
          <li
            :class='{active: currentIndex === index}'
            v-for='(item, index) in navList'
            :key='index'
          ><a href="">{{item}}</a></li>
        </ul>
        <div class="userLogin">
          <div class="login"><a href="">{{login}}</a></div>
          <div class="register"><a href="">{{register}}</a></div>
        </div>
      </div>
    </div>
    
  </div>

</template>

<script>
export default {
  name: 'navHead',
  data () {
    return {
      navList: ['首页','目的地','酒店','出游预定','旅游攻略'],
      login: '登录',
      register: '注册',
      show: false,
      currentIndex: 0
    }
  }
}
</script>

<style scoped lang='less'>
@import '../../assets/css/common.less';
  .navHead {
    width: 100%;
    height: 70px;
    box-shadow: 0 1px 1px 0 @BlackRgbO;
    &_container {
      width: 1200px;
      height: 100%;
      margin: 0 auto;
      .logo, .nav {
        display: inline-block;
      }
      .logo {
        float: left;
      }
      .nav {
        float: right;
        ul {
          display: inline-block;
          li {
            display: inline-block;
            width: 100px;
            height: 70px;
            line-height: 70px;
            color: #000;
            font-size: 16px;
            text-align: center;
            a {
              color: @Black;
            }
            &:hover {
              cursor: pointer;
              border-bottom: 3px solid @lightGreen;
            }
          }
          .active {
            background: @lightGreen;
            color: #fff;
            &:hover {
              border-bottom: 0px solid @lightGreen;
            }
            a {
              color: #fff;
            }
          }
        }
        .userLogin {
          display: inline-block;
          .login, .register {
            color: #000;
            font-size: 14px;
            padding: 10px 30px;
            border-radius: 4px; 
            display: inline-block;
            &:hover {
              cursor: pointer;
            }
          }
          .login {
            margin: 0 20px 0 40px;
            border: 1px solid @lightGreen;
            transition: all 400ms ease;
            a {
              color: @BlackRgb;
            }
            &:hover {
              opacity: 0.88;
              a {
                // transform: scale(1.2)
              }
            }
          }
          .register {
            background: @lightGreen;
            transition: all 400ms ease;
            a {
              color: #fff;
            }
            &:hover {
              opacity: 0.88;
            }
          }
        }
      }
    }
    
  }
</style>
