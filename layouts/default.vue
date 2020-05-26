<template>
  <div>
  <a-layout id="components-layout-demo-fixed">
    <a-layout-header :style="{ position: 'fixed', zIndex: 1, width: '100%',padding:0, background:'linear-gradient(#fff,#d4d7db)',boxShadow:'0 4px 4px rgba(0,0,0,.2)' }">
    <div class="header-line">
      
    </div>
      <div class="header-content">
        <div class="logo" />
      <a-menu
        theme="dark"
        mode="horizontal"
        :default-selected-keys="['2']"
        :style="{ lineHeight: '64px',background:'linear-gradient(#fff,#d4d7db)' }"
      >
        <a-menu-item key="1">
          nav 1
        </a-menu-item>
        <a-menu-item key="2">
          nav 2
        </a-menu-item>
        <a-menu-item key="3">
          nav 3
        </a-menu-item>
      </a-menu>
      </div>
      
    </a-layout-header>
    <a-layout-content :style="{ padding: '0 50px', margin: '80px auto 0 auto',width:'1200px', }">
      <div :style="{minHeight: '380px' }">
        <nuxt />
      </div>
    </a-layout-content>
    <a-layout-footer :style="{ textAlign: 'center' }">
      Ant Design ©2018 Created by Ant UED
    </a-layout-footer>
  </a-layout>
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
#components-layout-demo-fixed .logo {
  width: 120px;
  height: 31px;
  background: rgba(255, 255, 255, 0.2);
  margin: 16px 24px 16px 0;
  float: left;
}
.header-line{
  height: 2px;
  width: 100%;
  background: url(../assets/img/header_bj.gif) repeat-x;
}
.header-content{
  width: 1200px;
  height: 62px;
  overflow: hidden;
  margin:0 auto;
}
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
