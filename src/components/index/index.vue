<template>
  <el-container>
    <el-header>
      <header-layout></header-layout>
    </el-header>
    <el-main>
      <main-layout></main-layout>
    </el-main>
    <el-footer>
      <FooterLayout></FooterLayout>
    </el-footer>
  </el-container>
</template>

<script>
import HeaderLayout from '@/components/index/header/index'
import MainLayout from '@/components/index/main/index'
import FooterLayout from '@/components/index/footer/index'
export default {
  components: { MainLayout, HeaderLayout, FooterLayout },
  name: 'index',
  data () {
    return {
    }
  }
}
</script>
<style scoped>
  .el-header{
    color: #333;
    text-align: center;
    padding: 0px;
    height: 100px;
  }

  .el-main {
    color: #333;
    text-align: center;
    padding: 0px;
    margin-top: 30px;
  }

</style>
