<template>
  <div class="list">
    <div class="list_tab">
      <el-tabs v-model="activeName" @tab-click="handleClick">
        <el-tab-pane label="热门游记" name="first">热门游记</el-tab-pane>
        <el-tab-pane label="最新发表" name="second">最新发表</el-tab-pane>
      </el-tabs>
    </div>
    <div class="list_container">
      <ul>
        <li>
          <div class="left_con">
            <img src="" alt="">
          </div>
          <div class="right_con">
            <h2>天空之镜</h2>
            <p>时发生的纠纷年圣诞节</p>
            <div class="footer">
              <div class="footer_left">
                <i></i>
                <span>{{location}},</span>by<span>{{author}}</span>
              </div>
              <div class="footer_right">
                <span>25</span>
                <div class='icon'></div>
              </div>
            </div>
          </div>
        </li>
      </ul>
    </div>
    <div class="pageSize">

    </div>
  </div>

</template>

<script>
export default {
  name: 'list',
  data() {
    return {
      location: '宁乡',
    }
  },
}
</script>

<style>

</style>
