<template>
  <div class="home">
    <header-com class="header"></header-com>
    <left-com class="left"></left-com>
    <main-com class="main">dddd</main-com>
    <foot-com class="foot"></foot-com>
  </div>
</template>

<script>
  import HeaderCom from "./childcomponent/HeaderCom";
  import LeftCom from "./childcomponent/LeftCom";
  import MainCom from "./childcomponent/MainCom";
  import FootCom from "./childcomponent/FootCom";
  export default {
    name: 'Home',
    components: {
      HeaderCom,
      LeftCom,
      MainCom,
      FootCom
    },
    data() {
      return {
        tableData: null
      }
    }
  };
</script>


<style >
  .home{

  }
  .header {
    position: fixed;
    top: 0;
    right: 0;
    left: 0;

    width: 60px;
    background-color: #f2f2f2;
  }
  .header .left{
    position: fixed;
    top: 60px;
    left: 0;
    bottom: 0;
    /*background-color: aqua;*/
    /*background-color: rgba(0,0,0, 0.08);*/
    background-color: white;
    width: 20%;
    border: 1px solid #ddd;
  }
  .header .main{
    position: fixed;
    top: 60px;
    left: 20%;
    right: 0;
    bottom: 40px;
    width: 100%;
    background-color: aquamarine;
  }
  .header .foot{
    background-color: darkblue;
  }
</style>

