<template>
  <div class="home">
    <drawer-layout :drawerWidth="300" :triggerArea="0.2" btnId="enum">
      <div slot="drawer" class="slider">
        Login
        <h2 @click="$router.replace('/login')">登录</h2>
      </div>
      <div slot="content" class="main">
        <div id="enum">菜单</div>
        this is Context
      </div>
    </drawer-layout>
  </div>
</template>

<script>
// @ is an alias to /src
import {DrawerLayout} from "../components";

export default {
  name: 'Home',
  components:{
    DrawerLayout
  }
}
</script>
<style lang="less" scoped>
  .main {
    background: #fff;
    height: 100vh;
  }
  .slider {
    background: #42b983;
    height: 100vh;
  }
</style>
