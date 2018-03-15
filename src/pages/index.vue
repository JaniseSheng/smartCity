<template>
  <div class="" style="background-color: rgb(243, 243, 243); position: relative;">

      <div class="content-wrapper" >
        <div class="content-img">
          <div class="img-select-wrappr">
            <ButtonGroup>
               <Button size="large" :type="tabname == 1 ? 'primary' : 'default'" @click='tabname = 1'>物联网+城市管理</Button>
               <Button size="large" :type="tabname != 1 ? 'primary' : 'default'"  @click='tabname = 2'>小区进出影像采集</Button>
               <Button size="large" >小区消防通道地磁</Button>
           </ButtonGroup>
         </div>
         <transition name="slide-fade">
           <img v-show='tabname == 1' src="http://p5jbmbfmc.bkt.clouddn.com/img1.png" style="max-width: 100%; max-height: 100%" alt="">
         </transition>
        <transition name="slide-fade">
         <p v-show='tabname != 1' style="position: relative">
           <img  src="http://p5jbmbfmc.bkt.clouddn.com/img2.png" style="max-width: 100%; max-height: 100%" alt="">
           <span class='tabBtn3' @click='tabname = 3' :style="tabname == 3 ? 'box-shadow: 0 0 6px 3px #2b85e4;' : ''">
           </span>
         </p>
         </transition>
        </div>
        <div class="content-text">
          <div class="content-text-block">
            <transition name="text-fade">
              <div v-if='tabname == 1'>
                 <h2>
                   需求
                 </h2>
               <Form :label-width="40">
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                     集“物联、数联、智联”三位一体的驱动模式 ，构建新型智慧城市架构
                 </FormItem>
               </Form>
                 <h2 style='padding-top: 24px'>
                   优势
                 </h2>
               <Form :label-width="40">
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   上海电信已全面完成NB-IoT网络建设与整体覆盖
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   全球首个NB-IoT套餐
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   发布物联网开放平台
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   能够提供覆盖“终端、网络、服务”端到端的整体安全解决方案
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   提供基于国际认证的运维管理服务，并结合自身特点，建立了一套制度化、流程化、标准化的运营管理体系，同时拥有国内最强大、最专业的维护保障团队
                 </FormItem>
               </Form>
             </div>
            </transition>
            <transition name="text-fade">
              <div v-if='tabname == 2'>
                 <h2>
                   现状需求
                 </h2>
               <Form :label-width="40">
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                     小区入口传统监控系统技术落后、智能化水平低、资源利用率不足、维护量大。
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   大量流动人口涌入与平安城市监控管理之间的矛盾更加凸显。
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   缺乏对往来人员的记录和监督，导致事件发生后，难以取证。
                 </FormItem>
               </Form>

                 <h2 style='padding-top: 24px'>
                   解决方案
                 </h2>
               <Form :label-width="40">
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   人员车辆布控预警
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   动态人脸比对
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   轨迹查询
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   预案搜索
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   目标特征检索
                 </FormItem>
                 <FormItem>
                   <template slot='label'>
                     <Icon type="ios-circle-filled"></Icon>
                   </template>
                   以图搜图
                 </FormItem>
               </Form>
             </div>
            </transition>
            <transition name="text-fade">
              <div v-if='tabname == 3'>
                 <h2>
                   合作伙伴
                 </h2>

                 <h2 style='padding-top: 24px'>
                   产品 - (“深眸”人脸筒机)
                 </h2>
                 <Form :label-width="40">
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     Smart侦测
                   </FormItem>
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     Smart录像
                   </FormItem>
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     Smart编码
                   </FormItem>
                 </Form>
                 <h2 style='padding-top: 24px'>
                   产品 - (海康脸谱定位于系统)
                 </h2>
                 <Form :label-width="40">
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     人脸建模
                   </FormItem>
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     人脸特征识别
                   </FormItem>
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     黑名单功能
                   </FormItem>
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     1V1比对功能
                   </FormItem>
                 </Form>
                 <h2 style='padding-top: 24px'>
                   产品 - (人脸比对应用平台iVMS-8200-FAS)
                 </h2>
                 <Form :label-width="40">
                   <FormItem>
                     <template slot='label'>
                       <Icon type="ios-circle-filled"></Icon>
                     </template>
                     集实时抓拍与对比预警于一体
                   </FormItem>
                 </Form>
              </div>
            </transition>
          </div>
        </div>
      </div>

  </div>

</template>

<script>
export default {
  data(){
    return {
      tabname: 1
    }
  }
}
</script>


<style lang='less' scoped>
.content-wrapper {
  margin: auto;
  max-width: 1400px;
  height: 840px;
  &:after {
    content: '';
    display: table;
    clear: both;
  }
}
.content-img {
  width: 66.2%;
  float: left;
  height: 100%;
  padding: 96px 32px 32px ;
  text-align: center;
  position: relative;
}
.content-text {
  width: 33.8%;
  float: left;
  height: 100%;
  border-left: 1px dashed rgba(73, 198, 251, 0.69);
  position: relative;
}
.img-select-wrappr {
  position: absolute;
  top: 24px;
}
.content-text-block {
  position: relative;
  padding: 24px 12px;
  h2 {
    padding-bottom: 10px;
    color: #2d8cf0;
    border-bottom: 1px solid #2d8cf0;
  }

  :global(.ivu-form-item-content) {
    font-size: 15px !important;
  }
  :global(.ivu-form-item) {
    margin-bottom: 12px;
  }
}
.tabBtn3 {
  position: absolute;
  width: 35%;
  border: 2px solid;
  border-color: transparent;
  top: 10%;
  right: 0;
  bottom: 30%;
  box-shadow: 0 0 1px 2px rgba(153,153,153,0.6);
  transition: box-shadow .3s ease;
  cursor: pointer;
  &:hover {
    box-shadow: 0 0 6px 3px #2b85e4;
  }
}
/* 可以设置不同的进入和离开动画 */
/* 设置持续时间和动画函数 */
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .6s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active for below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}
.text-fade-enter-active {
  transition: all .3s ease;
}
.text-fade-leave-active {
  transition: all .6s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.text-fade-enter, .text-fade-leave-to
/* .slide-fade-leave-active for below version 2.1.8 */ {
  position: absolute;
  transform: translateY(10px);
  opacity: 0;
}
</style>
