<template>
  <div class="header">
    <div class="header-item item-left">
      <a href="/home" @click="">
        <img class="logo" src='../../assets/img/logo.png' alt="">
      </a>
    </div>
    <div class="header-item item-center">这是中间内容</div>

    <div class="header-item item-right">
      <el-dropdown>
        <span class="el-dropdown-link">
          <img class="profile-img" src="../../assets/img/logo.png" alt="">
          <i class="el-icon-arrow-down el-icon--right"></i>
        </span>
      <el-dropdown-menu slot="dropdown">
        <el-dropdown-item>个人信息</el-dropdown-item>
        <el-dropdown-item>更改密码</el-dropdown-item>
        <el-dropdown-item>退出</el-dropdown-item>
      </el-dropdown-menu>
      </el-dropdown>
    </div>
  </div>

</template>

<script>
  export default {
    name: "HeaderCom",
    computed: {
      avatar(){
        return '../../assets/img/logo.png'
      }
    }
  }
</script>

<style scoped>
  .header{
    /*display: flex;*/
    width: 100%;
    height: 60px;
    flex: 1;
  }
  .header .logo{
    padding: 10px 20px;
    width: 40px;
    height: 40px;
  }
  /*.header .header-item {*/
  /*  flex: 1;*/
  /*}*/
  .header .item-left {
     background-color: aquamarine;
     /*flex: 1;*/
     width: 20%;
     height: 100%;
     /*background-color: blue;*/
   }
  .header .item-left a:hover {
    cursor: pointer;
  }
  .header .item-center{
    height: 100%;
    text-align: center;
  }
  .header .item-right{
    position: fixed;
    top: 0;
    right: 0;
    height: 60px;
    width: 20%;

    padding-top: 10px;
    text-align: center;
  }
  .header .profile-img{
    width: 38px;
    height: 38px;
  }
</style>