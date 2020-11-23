<template>
  <div class="header">
    <div class="nav-topbar">
      <div class="container">
        <div class="topbar-menu"></div>
        <div class="topbar-user">
          <a hred="javascript:;">小米商城</a>
          <a hred="javascript:;">MUI</a>
          <a hred="javascript:;">云服务</a>
          <a hred="javascript:;">协议规则</a>
        </div>
      </div>
    </div>
    <div class="nav-header">
      <a hred="javascript:;">登录</a>
      <a hred="javascript:;">注册</a>
      <a hred="javascript:;">购物车</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "nav-header",
};
</script>
<style lang="scss">
  .header {
    height: 39px;
    line-height: 39px;
    .container {
      width:1226px;
      margin-right: auto;
      margin-left: auto;
    }
  }
</style>
