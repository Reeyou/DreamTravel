<template>
  <div class="banner">
    <div class='banner_img'>
      <ul>
        <li v-for='(item, index) in imgList' :key='index'>
          <img v-bind:src="item.url">
          <div class="descript">
            <h2>{{item.title}}</h2>
            <p>{{item.desc}}</p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'banner',
  data () {
    return {
      imgList: [
        {
          url: require('@/assets/img/banner_1.jpeg'),
          title: '金秋四月',
          desc: '迷人'
        },
        {
          url: require('@/assets/img/banner_2.jpeg'),
          title: '金秋四月',
          desc: '迷人'
        },
        {
          url: require('@/assets/img/banner_3.jpeg'),
          title: '【突然，南极】21岁，触碰世界另一端的冰冻星球',
          desc: '迷人'
        },
        {
          url: require('@/assets/img/banner_4.jpeg'),
          title: '金秋四月',
          desc: '迷人'
        },
        {
          url: require('@/assets/img/banner_5.jpeg'),
          title: '金秋四月',
          desc: '迷人'
        }
      ]
    }
  },
}
</script>

<style lang='less'>
  .banner {
    width: 100%;
    height: 500px;
    &_img {
      li {
        position: absolute;
        left: 0;
        top: 70px;
        z-index: -1;
        .descript {
          position: absolute;
          top: 100px;
          left: 100px;
          h2 {
            color: #fff;
            font-size: 50px;
            font-weight: 600;
          }
          p {
            color: #fff;
            font-size: 18px;
            font-weight: 500
          }
        }
      }
    }
  }
</style>
