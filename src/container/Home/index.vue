<template>
  <div>
    <nvHead />
    <Banner />
    <div class='container'>
      <List />
      <Side />
    </div>
    <Footer />
  </div>
</template>

<script>
import nvHead from '../../components/nav/header'
import Footer from '../../components/nav/footer'
import Banner from './Banner'
import List from './List'
import Side from './Side'
export default {
  name: 'Home', // 首页
  data() {
    return {

    }
  },
  components: {
    nvHead,
    Banner,
    List,
    Side,
    Footer
  }
}
</script>

<style>

</style>
