<template>
  <div>
    <nvHead />
    <Banner />
  </div>
</template>

<script>
import nvHead from '../../components/nav/header'
import Banner from '../../components/Banner'
export default {
  name: 'Home', // 首页
  data() {
    return {

    }
  },
  components: {
    nvHead,
    Banner
  }
}
</script>

<style>

</style>
