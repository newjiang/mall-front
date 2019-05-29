<template>
  <div class="header-style">
      <el-row :span="24" class="nav">
        <el-col :span="2">嗨，欢迎来到天猫</el-col>
        <el-col :span="1">请登陆</el-col>
        <el-col :span="1">免费注册</el-col>
        <el-col :span="10"><div class="temp"></div></el-col>
        <el-col :span="2" class="has-icon"><i class="el-icon-user-solid">我的</i></el-col>
        <el-col :span="2" class="has-icon"><i class="el-icon-shopping-cart-2">购物车</i></el-col>
        <el-col :span="2" class="has-icon"><i class="el-icon-star-on">收藏夹</i></el-col>
        <el-col :span="2" class="has-icon"><i class="el-icon-s-shop">商家支持</i></el-col>
        <el-col :span="2" class="has-icon"><i class="el-icon-menu">网站导航</i></el-col>
      </el-row>
      <el-row :span="24">
        <el-col :span="6"><div class="temp"></div></el-col>
        <el-col :span="12">
          <el-input placeholder="请输入内容" v-model="input" class="search">
            <el-button slot="append" icon="el-icon-search"></el-button>
          </el-input>
        </el-col>
        <el-col :span="6"><div class="temp"></div></el-col>
      </el-row>
  </div>
</template>

<script>
export default {
  name: '',
  data () {
    return {
      input: ''
    }
  }
}
</script>

<style scoped>
  .el-row{
    font-size: 12px;
    background-color: #ff0000;
  }
  .header-style{
    color: #ffffff;
  }
  .nav{
    text-align: right;
    padding-right: 3px;
    height: 20px;
    background-color: #ff0000;
    -webkit-box-shadow: #666 0px 0px 10px;
    -moz-box-shadow: #666 0px 0px 10px;
    box-shadow: #666 0px 0px 10px;
    z-index: 100;
  }
  .has-icon{
    margin-top: 2px;
  }
  .temp{
    border-radius: 4px;
    min-height: 1px;
  }
  .search{
    border-radius: 20px;
    margin-bottom: 15px;
    margin-top: 15px;
  }
</style>
