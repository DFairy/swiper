<template>
<div>
    <!-- <ul id="menu">
        <li data-menuanchor="page1" class="active"><a href="#page1">Section 1</a></li>
        <li data-menuanchor="page2"><a href="#page2">Section 2</a></li>
        <li data-menuanchor="page3"><a href="#page3">Section 3</a></li>
    </ul> -->
    <ul class='menu'>
        <li data-menuanchor="page1" class="active"><a href="#page1">热门游戏推荐</a></li>
        <li data-menuanchor="page2"><a href="#page2">游戏资讯</a></li>
        <li data-menuanchor="page3"><a href="#page3">游戏专区</a></li>
        <li data-menuanchor="page4"><a href="#page4">游戏下载</a></li>
    </ul>
    <!-- <ul class="actions">
        <li>
            <a class="actions-button" href="#" rel="noopener" @click="$refs.fullpage.api.moveSectionDown()">Move down</a>
        </li>
    </ul> -->

    <full-page ref="fullpage" :options="options" id="fullpage" >
        <div class="section">
            <!-- <home></home> -->
            <home></home>
        </div>
        <div class="section">
            <about></about>
        </div>
        <div class="section">
            <game></game>
        </div>
        <div class="section">
           <range></range>
        </div>
    </full-page>
</div>
</template>

<script>
import home from './Home'
import about from './About'
import game from './game'
import range from './range'
export default {
   components:{
      home,about,game,range
   },
  data: function(){
    return {
      options: {
        afterLoad: this.afterLoad,
        scrollBar: true,//侧边栏滚动条
        navigation: true,//分页指标
        menu: '#menu',
        anchors: ['page1', 'page2', 'page3','page4'],
      //   sectionsColor: ['#fff', '#fff', '#0798ec', '#fec401', '#1bcee6', '#ee1a59', '#2c3e4f']
      }
    }
  },
  methods: {
    afterLoad: function() {
      console.log('After load');
    }
  }
}
</script>

<style lang='less' scoped>
@import '../common/style/mixin.less';
 .menu{
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index:70;
    -webkit-font-smoothing:antialiased;
    -moz-font-smoothing:antialiased;
    letter-spacing:1px;
    .flex(flex-start);
    padding:10px 20px;
    padding-left: 20%; 
    background:rgba(0,0,0,0.5);
    li {
     padding: 0.5em 1em;
      cursor: pointer;
      position: relative;
      font-size:1em;
      color: #fff;
         &::after {
            content: "";
            width: 0;
            height: 2px;
            background-color: #ff6600;
            position: absolute;
            left: 100%;
            bottom: 0;
            transition: all .4s;
         }
         &:hover {
            &::after {
                  width: 100%;
                  left: 0;
                  transition-delay: 0.1s;
            }
            & ~ li::after {
                  left: 0;
            }
         }
         a{
            color: #fff;
            text-decoration: none;
            &:hover{
               color: #ff6600;
            }
         }
      }
   //  li{
   //     a{
   //       display: block;
   //       color: #fff;
   //       padding: 0.5em 1.2em;
   //       text-decoration: none;
   //       font-family: 'Play-Regular';
   //       font-size: 1em;
   //       &::after {
   //          content: "";
   //          width: 0;
   //          height: 2px;
   //          background-color: #00adb5;
   //          position: absolute;
   //          left: 100%;
   //          bottom: 0;
   //          transition: all .4s;
   //       }
   //       &:hover {
   //          color: #00adb5;
   //          &::after {
   //                width: 100%;
   //                left: 0;
   //                transition-delay: 0.1s;
   //          }
   //          & ~ a::after {
   //                left: 0;
   //          }
   //       }
   //     }
   //  }
 }
</style>