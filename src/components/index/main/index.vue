<template>
  <el-row>
    <el-col :span="4">
      <div class="main-left">
        <el-row>
          <el-menu
            background-color="#545c64"
            text-color="#fff"
            active-text-color="#ffd04b">
            <el-menu-item>图书、音像、数字商品</el-menu-item>
            <el-menu-item>家用电器</el-menu-item>
            <el-menu-item>手机、数码</el-menu-item>
            <el-menu-item>电脑、办公</el-menu-item>
            <el-menu-item>家居、家具、家装、厨具</el-menu-item>
            <el-menu-item>服饰内衣</el-menu-item>
            <el-menu-item>个护化妆</el-menu-item>
            <el-menu-item>运动健康</el-menu-item>
            <el-menu-item>汽车用品</el-menu-item>
            <el-menu-item>彩票、旅行</el-menu-item>
            <el-menu-item>理财、众筹</el-menu-item>
            <el-menu-item>母婴、玩具</el-menu-item>
            <el-menu-item>箱包</el-menu-item>
            <el-menu-item>运动户外</el-menu-item>
            <el-menu-item>箱包</el-menu-item>
          </el-menu>
        </el-row>
      </div>
    </el-col>
    <el-col :span="16">
      <div class="main-middle">
        <el-carousel :interval="5000" height="480px" arrow="always">
          <el-carousel-item v-for="item in 4" :key="item">
            <el-image :src="src"></el-image>
          </el-carousel-item>
        </el-carousel>
      </div>
    </el-col>
    <el-col :span="4">
      <div class="main-right">
        <el-row :span="24" style="height: 47px">
          <el-col :span="16" style="text-align: left;padding-left: 3px;padding-top: 5px">天猫活动</el-col>
          <el-col :span="8" style="text-align: right;padding-right: 3px;padding-top: 5px">更多></el-col>
        </el-row>
        <el-row :span="24" style="height: 35px">
          <el-col :span="24">[特惠]备战开学季 全民半价购数码</el-col>
        </el-row>
        <el-row :span="24" style="height: 35px">
          <el-col :span="24">[公告]备战开学季 全民半价购数码</el-col>
        </el-row>
        <el-row :span="24" style="height: 35px">
          <el-col :span="24">[公告]备战开学季 全民半价购数码</el-col>
        </el-row>
        <el-row :span="24" style="height: 35px">
          <el-col :span="24">[公告]备战开学季 全民半价购数码</el-col>
        </el-row>
        <el-row :span="24" style="height: 35px">
          <el-col :span="24">[公告]备战开学季 全民半价购数码</el-col>
        </el-row>
        <el-row :span="24">
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
        </el-row>
        <el-row :span="24">
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
          <el-col :span="6">
            <i class="el-icon-platform-eleme"/>
            <p>饿了么</p>
          </el-col>
        </el-row>
        <el-row :span="24" style="height: 30px">
          <el-image :src="icon"></el-image>
        </el-row>
      </div>
    </el-col>
  </el-row>
</template>

<script>
export default {
  name: 'layout1',
  data () {
    return {
      src: 'https://cube.elemecdn.com/6/94/4d3ea53c084bad6931a56d5158a48jpeg.jpeg',
      icon: 'http://k.zol-img.com.cn/sjbbs/7692/a7691515_s.jpg'
    }
  }
}
</script>

<style scoped>
  .el-menu {
    background: #aaaaaa;
  }
  .main-left{
    background: #cccccc;
  }
  .main-right{
    font-size: 12px;
  }

  .el-menu-item {
    text-align: left;
    height: 32px;
    line-height: 32px;
  }

</style>
