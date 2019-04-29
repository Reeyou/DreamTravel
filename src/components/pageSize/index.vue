<template>
  <div 
    class="pageSize"
    :pages='pages'
    :currentPage='currentPage'
    :totalPage='totalPage'
  >
    <div class="total">
      <span></span>/<span></span>
    </div>
    <div class="prev"></div>
    <div class="pages">
      <ul>
        <li></li>
      </ul>
    </div>
    <div class="next"></div>
    <div class='jump'>
      <input type="text">
      <span>跳转</span>
    </div>
  </div>

</template>

<script>
export default {
  name: 'pageSize', // list内容分页
  props: ['totalPage', 'currentPage'],
  data() {
    return {

    }
  },
}
</script>

<style>

</style>
