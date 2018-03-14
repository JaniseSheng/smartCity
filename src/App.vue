<template>
<div id="app">
  <div class="menu-wrapper">
    <div class="menu-block">
      <p data-type='title-name'>
        <Icon type="earth" />
        智能知识库
      </p>
      <p class='menu-item-wrapper'>
        <Menu mode="horizontal" :theme="theme" active-name="1">
          <MenuItem name="1">
              <Icon type="ios-paper"></Icon>
              解决方案
          </MenuItem>
          <MenuItem name="2">
              <Icon type="ios-people"></Icon>
              知识搜索
          </MenuItem>
          <MenuItem name="3">
              <Icon type="ios-people"></Icon>
              知识图谱
          </MenuItem>
          <MenuItem name="4">
              <Icon type="settings"></Icon>
              我的偏好
          </MenuItem>
      </Menu>
      </p>
    </div>

  </div>
  <router-view></router-view>
</div>
</template>

<script>
 export default {
   data(){
     return {
       theme: 'light'
     }
   }
  }
</script>
<style lang='less' scoped>
.menu-wrapper {
  position: relative;
  
}
.menu-block {
  & [data-type='title-name'] {
    font-size: 18px;
  }
}
.menu-item-wrapper {
  & .ivu-menu:after {
    display: none;
  }
  & .ivu-menu-item {
    border-bottom: none !important;
  }
}
</style>
