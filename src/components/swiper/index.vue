<template>
  <div class="swiper">
    <div class="container">
      <ul>
        <li
          v-for='(item, index) in swiperList'
          :key=index
        >
          <img :src="item.url" :alt="item.desc">
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'swiper', // banner轮播
  props: ['imgList'],
  data() {
    return {
      swiperList: imgList
    }
  },
}
</script>

<style scoped lang='less'>

</style>
