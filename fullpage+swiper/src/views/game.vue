<template>
   <div class='game'>
       <div class='menu'>
           <b>游戏类型:</b>
           <ul class="tabs">
                <li class="tab-item" v-for="(item,index) in menu" :key='index'
                :class="{active:isActive==index}"
                @click="choose(index)"
               >{{item.title}}
                </li>
            </ul>
       </div>
       <div>
           <ul class='game-list'>
               <li>
                   <img src="../common/img/1.jpg" alt="">          
                   <div class='content'>
                       <p class='title'><a href="javascript:void(0)">最牛的游戏</a> <button class="btn">游戏下载</button></p>
                       <div class="hot blue">
							<a href="javascript:void(0)" target="_blank" title="">单机</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">角色扮演</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">休闲</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">毁三观</a>
						</div>
                        <p class='detail'>
                            《模拟山羊》是一部荒诞的游戏，而这大概也是人们唯一能够在其身上确定的特质。
                            主角是一只无节操，没大脑，整天要死要活的山羊,玩家要控制这只山羊在一个模拟的世界中冒险，制作各种机会让山羊得偿所愿，
                        </p>
                   </div>
                   <div class='rate'><div><i>5.0</i><span>分</span></div></div>
               </li>
                <li>
                   <img src="../common/img/1.jpg" alt="">          
                   <div class='content'>
                       <p class='title'><a href="javascript:void(0)">最牛的游戏</a> <button class="btn">游戏下载</button></p>
                       <div class="hot blue">
							<a href="javascript:void(0)" target="_blank" title="">单机</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">角色扮演</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">休闲</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">毁三观</a>
						</div>
                        <p class='detail'>
                            《模拟山羊》是一部荒诞的游戏，而这大概也是人们唯一能够在其身上确定的特质。
                            主角是一只无节操，没大脑，整天要死要活的山羊,玩家要控制这只山羊在一个模拟的世界中冒险，制作各种机会让山羊得偿所愿，
                        </p>
                   </div>
                   <div class='rate'><div><i>5.0</i><span>分</span></div></div>
               </li>
                <li>
                   <img src="../common/img/2.jpg" alt="">          
                   <div class='content'>
                       <p class='title'><a href="javascript:void(0)">最牛的游戏</a> <button class="btn">游戏下载</button></p>
                       <div class="hot blue">
							<a href="javascript:void(0)" target="_blank" title="">单机</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">角色扮演</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">休闲</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">毁三观</a>
						</div>
                        <p class='detail'>
                            《模拟山羊》是一部荒诞的游戏，而这大概也是人们唯一能够在其身上确定的特质。
                            主角是一只无节操，没大脑，整天要死要活的山羊,玩家要控制这只山羊在一个模拟的世界中冒险，制作各种机会让山羊得偿所愿，
                        </p>
                   </div>
                   <div class='rate'><div><i>5.0</i><span>分</span></div></div>
               </li>
                <li>
                   <img src="../common/img/3.jpg" alt="">          
                   <div class='content'>
                       <p class='title'><a href="javascript:void(0)">最牛的游戏</a> <button class="btn">游戏下载</button></p>
                       <div class="hot blue">
							<a href="javascript:void(0)" target="_blank" title="">单机</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">角色扮演</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">休闲</a>
							<em>+</em>
							<a href="javascript:void(0)" target="_blank" title="">毁三观</a>
						</div>
                        <p class='detail'>
                            《模拟山羊》是一部荒诞的游戏，而这大概也是人们唯一能够在其身上确定的特质。
                            主角是一只无节操，没大脑，整天要死要活的山羊,玩家要控制这只山羊在一个模拟的世界中冒险，制作各种机会让山羊得偿所愿，
                        </p>
                   </div>
                   <div class='rate'><div><i>5.0</i><span>分</span></div></div>
               </li>
           </ul>
           <div class='pagination'> <b-pagination v-model="currentPage" :total-rows="rows" size="sm"></b-pagination></div>
       </div>
   </div>
</template>

<script>
export default {
    data(){
        return{
            rows: 100,
            currentPage: 1,
            isActive: 0,
            menu:[
                {
                    title:'全部'
                },
                {
                    title:'益智解谜'
                },
                {
                    title:'动作游戏'
                },
                {
                    title:'角色扮演游戏'
                },
                {
                    title:'休闲游戏'
                },
                {
                    title:'策略游戏'
                },
                {
                    title:'体育'
                }
            ]
        }
    },
    methods:{
        choose(index){
            this.isActive=index
        }
    }
}
</script>

<style lang='less' scoped>
@import '../common/style/mixin.less';
.game{
    width: 100%;
    height: 100%;
    padding: 80px;
    .menu{
        font-size: 14px;
        .flex(flex-start);
        align-items: center;
        b{
            font-weight: 700;
            color: #585858;
            margin-right: 20px;
        }
        .tabs{
            padding-top: 5px;
            li{
                display: inline-block;
                font-weight: 500;
                padding: 5px 15px;
                color: #585858;
                text-decoration: none;
                overflow: hidden;
                border-radius: 2px;
                transition: all 0.2s linear;
                background: #f0f0f0;
                margin-left: 12px;
                font-size: 12px;
                cursor: pointer;
                &:hover{
                    background:#ff6600;
                    color: #fff;
                }
            }
            .active{
                background:#ff6600;
                color: #fff;
                position: relative;
                padding:5px 20px 5px 10px;
                &:before{
                    content: '';
                    position: absolute;
                    width: 12px;
                    height: 6px;
                    background: transparent;
                    top: 11px;
                    right: 2px;
                    border: 2px solid #fff;
                    border-top: none;
                    border-right: none;
                    -webkit-transform: rotate(-55deg);
                    -ms-transform: rotate(-55deg);
                    transform: rotate(-55deg);
                    z-index: 9;
                }
            }
        }
    }
    .game-list{
        margin-top: 20px;
        border-top:1px solid #ccc;
        li{
            .flex(space-between);
            align-items:flex-start;
            border-bottom:1px solid #ccc;
            padding: 20px 0;
            img{
                display: inline-block;
                width: 114px;
                height: 114px;
                border-radius: 5px;
            }
            .rate{
                width: 100px;
                height: 100px;
                border:5px solid #e6c515;
                border-radius: 50%;
                font-size: 30px;
                color: #7e7e7e;
                font-weight: bold;
                font-style: italic;
                .center;
                span{
                    font-size: 14px;
                    font-weight: bold;
                    padding-left: 5px;
                }
            }
            .content{
                flex:1;
                height: 100%;
                padding: 0 20px;
                .title{
                    width: 260px;
                    padding-right: 20px;
                    height: 31px;
                    line-height: 31px;
                    overflow: hidden;
                    font-size: 18px;
                    margin-bottom: 3px;
                    a{
                        color: #585858;
                        text-decoration: none;
                        font-weight: 500;
                        &:hover{
                            color: #ff6600;
                        }
                    }
                }
                .hot{
                    width: 280px;
                    height: 26px;
                    line-height: 26px;
                    font-size: 12px;
                    overflow: hidden;
                    text-decoration: none;
                    margin-bottom: 3px;
                    a{
                        color: #11c454;
                    }
                    em {
                        color: #dfdfdf;
                        font-style: normal;
                        padding: 0px 7px;
                    }
                }
                .detail{
                    width: 100%;
                    height: 40px;
                    font-size: 12px;
                    line-height: 22px;
                    overflow: hidden;
                }
                .btn{
                    width: 100px;
                    padding: 2px 15px;
                    text-align: center;
                    position: relative;
                    appearance: none;
                    background: #ff6600;
                    border: none;
                    color: white;
                    font-size: 14px;
                    cursor: pointer;
                    outline: none;
                    overflow: hidden;
                    border-radius: 100px;
                    margin-left: 20px;
                    margin-top: -5px;
                }
            }
        }
    }
    .pagination{
        .flex(flex-end);
        padding:20px; 
    }
}
</style>