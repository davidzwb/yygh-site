<template>
  <div class="app-container">
    <div id="main">
      <!-- 公共头 -->
      <MyHeader />
      <div class="main-container">
        <el-scrollbar class="page-component scroll">
          <!-- 内容区域 -->
          <nuxt />
        </el-scrollbar>
      </div>
      <!-- 公共底 -->
      <MyFooter />
    </div>
  </div>
</template>
<script>
import '~/assets/css/app.css'
import '~/assets/css/chunk.css'
import '~/assets/css/iconfont.css'
import '~/assets/css/main.css'
import MyHeader from './myheader'
import MyFooter from './myfooter'

export default {
  name: 'DefaultLayout',
  components: {
    MyHeader, MyFooter
  }
}
</script>