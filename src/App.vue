<template>
<div id="app" style="min-width: 1200px;">
  <div class="menu-wrapper">
    <div class="menu-block">
      <p class='menu-item-wrapper' style="background-color: #fff">
        <Menu mode="horizontal" :theme="theme" active-name="1" style="max-width: 1200px; margin: auto">
          <MenuItem name="1" class='menu-title'>
              <Icon type="earth"></Icon>
              智能知识库
          </MenuItem>
          <MenuItem name="1">
              <Icon type="ios-paper"></Icon>
              解决方案
          </MenuItem>
          <MenuItem name="2">
              <Icon type="android-search"></Icon>
              知识搜索
          </MenuItem>
          <MenuItem name="3">
              <Icon type="bookmark"></Icon>
              知识图谱
          </MenuItem>
          <MenuItem name="4">
              <Icon type="android-star"></Icon>
              我的偏好
          </MenuItem>
      </Menu>
      </p>
      <div style="max-width: 1200px; margin: auto; padding: 24px">
        <div class="title-info">
          <p style="font-size: 36px;">物联网 ---智慧城市解决方案</p>
          <p style="font-size: 20px;">集“物联、数联、智联”三位一体的驱动模式 ，构建新型智慧城市架构</p>
        </div>
      </div>
    </div>
  </div>
  <div class="tab-menu-wrapper">
    <div data-type='item' data-active='active'>
      <Icon type="social-buffer" style='font-size: 42px; padding-bottom: 12px;'></Icon>
      <p>通用架构解读</p>
    </div>
    <div data-type='item'>
      <Icon type="earth" style='font-size: 42px; padding-bottom: 12px;'></Icon>
      <p>经典应用场景</p>
    </div>
    <div data-type='item'>
      <Icon type="ios-book" style='font-size: 42px; padding-bottom: 12px;'></Icon>
      <p>技术解决方案</p>
    </div>
  </div>
  <router-view></router-view>
  <div style="padding: 24px; color:#2d8cf0; text-align: center">
    中国电信公司政企知识库
  </div>
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
  height: 400px;
  background-size: cover;
  background-image: url('http://p5jbmbfmc.bkt.clouddn.com/smartcity.jpg');
}
.menu-block {
  & [data-type='title-name'] {
    font-size: 18px;
  }
}
.menu-title {
  font-size: 20px;
  padding-right: 60px;
}
.menu-item-wrapper {
  & .ivu-menu:after {
    display: none;
  }
  & .ivu-menu-item {
    border-bottom: none !important;
  }
}
.title-info {
  padding-top: 80px;
  color: white;
  font-weight: bold;
}
.tab-menu-wrapper {
  max-width: 1400px;
  padding: 24px;
  margin: auto;
  &:after {
    content: '';
    clear: both;
    display: table;
  }
  & [data-type='item'] {
    float: left;
    width: 33.33%;
    text-align: center;
    font-size: 20px;
    &:nth-last-of-type(n + 2) {
      border-right: 1px solid #666;
    }
  }
  & [data-active='active'] {
    color: #2d8cf0
  }
}
</style>
