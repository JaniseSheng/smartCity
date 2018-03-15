<template>
  <div class="" style="background-color: rgb(243, 243, 243); position: relative;">

      <div class="content-wrapper" >
        <div class="content-img">
          <div class="img-select-wrappr">
            <ButtonGroup>
               <Button size="large" type="primary">物联网+城市管理</Button>
               <Button size="large" >小区进出影像采集</Button>
               <Button size="large">小区消防通道地磁</Button>
           </ButtonGroup>
         </div>
         <template v-if='tabname == 1'>
           <img src="http://p5jbmbfmc.bkt.clouddn.com/img1.png" style="max-width: 100%; max-height: 100%" alt="">
         </template>
        </div>
        <div class="content-text">
          <div class="content-text-block">
            <template v-if='tabname == 1'>
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

            </template>
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
</style>
