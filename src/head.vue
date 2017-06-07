<template>
	<header class="d-box headBar p_fixed bg_blue HomeheadBar">
      <aside class="pl_15 ta_avC b-flex">
        <a class="btnBox headBarLogo" href="javascript:;">
          <span class="fz_16 c_fff">
            <img v-bind:src="logo" alt="">
          </span>
        </a>
      </aside>
      <aside class="pr_15 ta_avC">
        <a class="btnBox" href="javascript:;">
          <i class="iconfont wf-bookshelf fz_18"></i>
        </a>
        <a class="btnBox" href="javascript:;">
          <i class="iconfont wf-search fz_18"></i>
        </a>
        <a class="btnBox" href="javascript:;">
          <i class="icon i-user hide mt_10"></i><!-- 未登录状态 -->
          <i class="icon i-userSign  mt_10"></i><!-- 已登录状态 -->
        </a>
      </aside>
  </header>
</template>
<style>
.headBar {width:100%;height:44px;position: absolute;position:fixed;top:0;left:0;font-size: 0;background-color:#ffffff;z-index:20;border-bottom: 1px solid #d9d9d9;}
 @media screen and (max-width: 320px) {
    .headBar-title .userAccount {
        max-width: 68px;
    }
 }
.headBar-title {height:100%;font-size:16px;line-height:44px;text-align:center;}
.headBar .wf-home{font-size:16px;}
.headBar_NoRight aside{width:43px;}
.headBar .wf-arrowL,.headBar .wf-bookadd,.headBar .wf-bookshelf,.headBar .wf-search{font-size:20px;}
.headBar .wf-home{font-size:22px;}
.headBar section .headBar-title{color: #1d232c;}
.headBarLogo{padding-top:6px;}
.headBarLogo img{height:26px;}
.headBar .TxtBtn{display: inline-block;width:29px;height: 28px;font-size: 14px;text-align:center;padding-top: 7px;color: #218eed;}
.HomeheadBar{border-bottom:none;}
.HomeheadBar .wf-bookshelf,.headBar .wf-search{color:#ffffff}
.HomeheadBar .pr_15 .btnBox{width:40px;height:44px;line-height:44px;text-align:center;display:block;}
.headBar .NovelNav .btnBox{width: 40px;height: 44px;line-height: 44px;text-align: center;display:block;}
.headBar .NovelNavD .btnBox{width: 32px;height: 44px;line-height: 44px;text-align: center;display:block;}
.personCenter .userImg{padding-top:8px;}
.personCenter .userImg img{width:26px;height:26px;border-radius:50%;}
</style>
<script>
    export default {
      data: function() {
        return {logo:'http://zhangxin.mail.10086.cn/html5/images/logo.png'}
      },
   	  methods:{

   	  }
    }
</script>