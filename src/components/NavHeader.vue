<template>
  <div class="header">
    <div class="nav-topbar">
      <div class="container">
        <div class="topbar-menu">
          <a hred="javascript:;">小米商城</a>
          <a hred="javascript:;">MUI</a>
          <a hred="javascript:;">云服务</a>
          <a hred="javascript:;">协议规则</a>
        </div>
        <div class="topbar-user">
          <a hred="javascript:;">登录</a>
          <a hred="javascript:;">注册</a>
          <a hred="javascript:;" class="my-cart"
            ><span class="icon-cart"></span>购物车</a
          >
        </div>
      </div>
    </div>
    <div class="nav-header">
      <div class="container">
        <div class="header-logo">
          <a href="#"></a>
        </div>
        <div class="header-menu">
          <div class="item-meun">
            <span>小米手机</span>
            <div class="childen">

            </div>
          </div>
          <div class="item-meun">
            <span>RedMi红米</span>
            <div class="childen"></div>
          </div>
          <div class="item-meun">
            <span>电视</span>
            <div class="childen"></div>
          </div>
        </div>
        <div class="header-search">
          <div class="wrapper">
            <input type="text" name="keyword" />
            <a href="javascript:;"></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "nav-header",
};
</script>
<style lang="scss">
// @import "./../assets/scss/base.scss";
.header {
  .nav-topbar {
    height: 39px;
    line-height: 39px;
    background-color: #333333;
    color: #b0b0b0;
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 1226px;
      margin-right: auto;
      margin-left: auto;
      a {
        display: inline-block;
        margin-right: 17px;
      }
      .my-cart {
        width: 110px;
        background-color: #ff6600;
        text-align: center;
        color: #ffffff;
        margin-right: 0;
        .icon-cart {
          display: inline-block;
          width: 16px;
          height: 12px;
          background: url("/imgs/icon-cart-checked.png") no-repeat center;
          background-size: contain;
          margin-right: 4px;
        }
      }
    }
  }
  .nav-header {
    .container {
      height: 112px;
      display: flex;
      width: 1226px;
      margin-right: auto;
      margin-left: auto;
      justify-content: space-between;
      align-items: center;
      .header-logo {
        display: inline-block;
        width: 55px;
        height: 55px;
        background-color: #ff6600;
        a {
          display: inline-block;
          width: 110px;
          height: 55px;
          &::before {
            content: " ";
            display: inline-block;
            width: 55px;
            height: 55px;
            background: url("/imgs/mi-logo.png") no-repeat center;
            background-size: 55px;
            transition: margin 0.2s;
          }
          &:after {
            content: " ";
            display: inline-block;
            width: 55px;
            height: 55px;
            background: url("/imgs/mi-home.png") no-repeat center;
            background-size: 55px;
            // @include bgImg(55px, 55px, "/imgs/mi-home.png", 55px);
          }
          &:hover:before {
            margin-left: -55px;
            transition: margin 0.2s;
          }
        }
      }
      .header-menu {
        display: inline-block;
        width: 643px;
        padding-left: 209px;
        .item-meun {
          display: inline-block;
          color: #333333;
          font-weight: bold;
          font-size: 16px;
          line-height: 112px;
          margin-right: 20px;
          span {
            cursor: pointer;
          }
        }
      }
    }
    .header-search {
      width: 319px;
      .wrapper {
        height: 50px;
        border: 1px solid #e0e0e0;
        display: flex;
        align-items: center;
        input {
          border:none;
          box-sizing: border-box;
          border-right: 1px solid #E0E0E0;
          width: 264px;
          height: 50px;
          padding-left: 14px;
        }
        a {
          display: inline-block;
          width: 18px;
          height: 18px;
          background: url("/imgs/icon-search.png") no-repeat center;
          background-size: contain;
          margin-left: 14px;
        }
      }
    }
  }
}
</style>
