<template>
   <div class='about'>
     <div class='game-left'>
       <ul class='game-list'>
         <li>
           <p class="title">《龙OL》今日两点重生公测，重铸活动经典重燃</p>
           <div class='content'>
             <div class='content-lf'>
               <img src="../common/img/1.jpg" alt="">
               <p>上海绿岸网络代理的经典客户端网游《龙OL》已于2019年5月15日14：00开启不删档重生公测。为了让新老用户重新拥抱新生的龙世界开服之际推出了用户回归、双倍经验以及海量充值道</p>
             </div>
             <div class='content-rt'>
                <div class='time'>2019-05-1511:29:18</div>
                <div>来自:<span>新网游</span></div>
             </div>
           </div>
         </li>
         <li>
           <p class="title">《龙OL》今日两点重生公测，重铸活动经典重燃</p>
           <div class='content'>
             <div class='content-lf'>
               <img src="../common/img/1.jpg" alt="">
               <p>上海绿岸网络代理的经典客户端网游《龙OL》已于2019年5月15日14：00开启不删档重生公测。为了让新老用户重新拥抱新生的龙世界开服之际推出了用户回归、双倍经验以及海量充值道</p>
             </div>
             <div class='content-rt'>
                <div class='time'>2019-05-1511:29:18</div>
                <div>来自:<span>新网游</span></div>
             </div>
           </div>
         </li>
         <li>
           <p class="title">《龙OL》今日两点重生公测，重铸活动经典重燃</p>
           <div class='content'>
             <div class='content-lf'>
               <img src="../common/img/1.jpg" alt="">
               <p>上海绿岸网络代理的经典客户端网游《龙OL》已于2019年5月15日14：00开启不删档重生公测。为了让新老用户重新拥抱新生的龙世界开服之际推出了用户回归、双倍经验以及海量充值道</p>
             </div>
             <div class='content-rt'>
                <div class='time'>2019-05-1511:29:18</div>
                <div>来自:<span>新网游</span></div>
             </div>
           </div>
         </li>
       </ul>
       <div class='pagination'> <b-pagination v-model="currentPage" :total-rows="rows" size="sm"></b-pagination></div>
      
     </div>
     <div class='game-right'>
       <div style="margin-bottom:20px;">
          <p class="title">
            <b>手游热点</b>
          </p>
          <ul class='news-list'>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
          </ul>
       </div>

        <div>
          <p class="title">
            <b>端游热点</b>
          </p>
          <ul class='news-list'>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
            <li>
              <a href=""><em></em>奇幻策略游戏《西娅2：粉碎》登陆Steam</a>
            </li>
          </ul>
       </div>
       
     </div>
   </div>
</template>

<script>

export default {
   data(){
      return{
            rows: 100,
            currentPage: 1,
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
        }
    }
}
</script>

<style lang='less' scoped>
@import '../common/style/mixin.less';
.about{
   width: 100%;
   height: 100%;
   padding: 80px;
  //  border: 1px solid red;
   .flex(flex-start);
   .game-left{
     height: 100%;
    //  border: 1px solid red;
     flex:1;
     .game-list{
       li{
         margin-bottom: 25px;   
         .title{
           font-size: 1.17em;
           font-weight: bold;
         }
         .content{ 
          //  margin-top: 20px;
           padding: 10px;
           font-size: 14px;
           color: #666565;
           .content-lf{
            //  border: 1px solid green;
             .flex(flex-start);
             align-items:flex-start;
             margin-bottom: 10px;
             img{
               width:200px;
               margin-right: 20px;
               border-radius: 5px;
             }
             p{
               line-height: 26px;
                
                font-size: 14px;
             }
           }
           .content-rt{
            //  border: 1px solid green;
            .flex(flex-start);
            .time{
              width: 220px;
            }
           }
         }
       }
     }
     .pagination{
        .flex(flex-end);
        padding-right:20px; 
      }
   }
   .game-right{
     height: 100%;
    //  border: 1px solid red;
     width: 300px;
     padding: 10px;
     .title{
        height: 48px;
        line-height: 48px;
        border-top: 1px solid #e7e7e7;
        margin-bottom: 8px;
        b{
          font-size: 18px;
          display: inline-block;
          border-top: 2px solid #ff6600;
          position: relative;
          top: -1px;
          font-weight: bold;
          color: #ff6600;
        }   
     }
     .news-list{
       li{
         width: 100%;
         height: 32px;
         line-height: 32px;
         white-space: nowrap;
         text-overflow: ellipsis;
         overflow: hidden;
         font-size: 14px;
         a{
           color: #474747;
           font-weight: 400;
           &:hover{
             color: #ff6600;
             text-decoration: none;
           }
           em{
              display: inline-block;
              width: 4px;
              height: 4px;
              background: #d5d5d5;
              vertical-align: middle;
              margin-right: 7px;
           }
         }
       }
     }

   }
}
</style>
