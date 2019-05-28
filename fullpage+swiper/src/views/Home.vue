<template>
   <div class='home'>
      <div class="swiper-container">
        <div class="swiper-wrapper" >
          <div class="swiper-slide" v-for="(item,index) in title" :key='index' :style="{backgroundImage:'url('+item.imgSrc+')'}">
              <div class="bottom">
                <p>{{item.title1}}</p>
                <p>{{item.title2}}</p>
              </div>
          </div>
          <!-- <div class="swiper-slide" style="background-image:url(http://lorempixel.com/600/600/nature/2)"></div>
          <div class="swiper-slide" style="background-image:url(http://lorempixel.com/600/600/nature/3)"></div>
          <div class="swiper-slide" style="background-image:url(http://lorempixel.com/600/600/nature/4)"></div>
          <div class="swiper-slide" style="background-image:url(http://lorempixel.com/600/600/nature/5)"></div> -->
        </div>
        <!-- Add Pagination -->
        <div class="swiper-pagination"></div>
      </div>
   </div>
</template>

<script>
import Swiper from "swiper";
import "swiper/dist/css/swiper.min.css";
export default {
   data(){
      return{
            title:[
                {
                    href:'',
                    title1:'主打推荐',
                    title2:'和平精英',
                    title3:'升级精英手册 享专属赛季奖励',
                    imgSrc:require('../common/img/1.jpg')
                },
                {
                    href:'',
                    title1:'重磅更新',
                    title2:'和平精英',
                    title3:'选择你的潜伏命运',
                    imgSrc:require('../common/img/2.jpg')
                },
                {
                    href:'',
                    title1:'重磅更新',
                    title2:'和平精英',
                    title3:'选择你的潜伏命运',
                    imgSrc:require('../common/img/3.jpg')
                },
                {
                    href:'',
                    title1:'重磅更新',
                    title2:'和平精英',
                    title3:'选择你的潜伏命运',
                    imgSrc:require('../common/img/4.jpg')
                },
                {
                    href:'',
                    title1:'重磅更新',
                    title2:'和平精英',
                    title3:'选择你的潜伏命运',
                    imgSrc:require('../common/img/3.jpg')
                },
                {
                    href:'',
                    title1:'重磅更新',
                    title2:'和平精英',
                    title3:'选择你的潜伏命运',
                    imgSrc:require('../common/img/4.jpg')
                },
                
            ],
      }
   },
    mounted(){
      this.init()
    },
    methods:{
        init(){
             /* eslint-disable */
            var mySwiper = new Swiper('.swiper-container', {
                  // loop: true,
                  // autoplay: {
                  //     delay:30000, 
                  //     disableOnInteraction: false,  //触碰后自动切换停止
                  // },
                //   paginationClickable :true,
                //   pagination: {
                //     el: '.swiper-pagination',
                //     clickable: true // 允许点击小圆点跳转
                //   },
                  // autoplayDisableOnInteraction: false,
                  // observer: true, //修改swiper自己或子元素时，自动初始化swiper
                  // observeParents: true,//修改swiper的父元素时，自动初始化swiper
                  // centeredSlides : true,
                  // slidesPerView:4,
                  initialSlide : 3,
                  effect: 'coverflow',
                  grabCursor: true,
                  centeredSlides: true,
                  slidesPerView: 'auto',
                  coverflowEffect: {
                    rotate: 50,
                    stretch: 0,
                    depth: 100,
                    modifier: 1,
                    slideShadows : true,
                  },
                  pagination: {
                    el: '.swiper-pagination',
                  },
            })
        }
    }
}
</script>

<style lang='less' scoped>
@import '../common/style/mixin.less';
.home{
   width: 100%;
   height: 100%;
   background: url('../common/img/3.jpg') no-repeat center center;
   padding: 80px;
   .center;
   .swiper-container {
      width: 100%;
      padding-top: 50px;
      padding-bottom: 50px;
    }
    .swiper-slide {
      background-position: center;
      background-size: cover;
      width: 300px;
      height: 400px;
      border-radius: 10px;
      overflow: hidden;
      .bottom{
        width: 100%;
        position: absolute;
        bottom: 0;
        left: 0;
        background: #fff;
        text-align: center;
        padding: 5px;
        font-size: 16px;
        color: #000;
      }
    }
   
}
</style>
