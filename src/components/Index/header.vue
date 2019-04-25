<template>
  <div class='navHead'>
    <div class='navHead_container'>
      <div class="logo">
        <img src="" alt="">
      </div>
      <div class="nav">
        <ul v-for='(item, index) in navList' :key='index'>
          <li>{item}</li>
        </ul>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'navHead',
  data() {
    return {
      navList: ['首页','目的地','酒店','出游预定','旅游攻略']
    }
  },
}
</script>

<style>

</style>
