<template>
    <div class="headMenu">
        <div class="menu">
            <ul class="clearfix" id="channel-nav">
                <div class="lavalamp-object"></div>
                <li class=" menu-index menu-item current active">
                    <a href="/">主页</a></li>
                <li class=" menu-item">
                    <router-link to="/guonei">国内</router-link>
                </li>
                <li class=" menu-item"><a href="#">国际</a></li>
                <li class=" menu-item"><a href="#">军事</a></li>
                <li class=" menu-item"><a href="#">财经</a></li>
                <li class=" menu-item"><a href="#">娱乐</a></li>
                <li class=" menu-item"><a href="#">体育</a></li>
                <li class=" menu-item"><a href="#">互联网</a></li>
                <li class=" menu-item"><a href="#">科技</a></li>
                <li class=" menu-item"><a href="#">游戏</a></li>
                <li class=" menu-item"><a href="#">女人</a></li>
                <li class=" menu-item"><a href="#">汽车</a></li>
                <li class=" menu-item"><a href="#">房产</a></li>
                <li class=" menu-item"><a href="#">国内</a></li>
                <li class=" menu-item"><a href="#" class="person">个性推荐</a></li>


                
            </ul>
        </div>
    </div>
</template>


<script>
import "../assets/libs/lavalamp/css/jquery.lavalamp.css";
import "../assets/libs/jquery.min.js";
import "../assets/libs/lavalamp/js/jquery.lavalamp.min.js";

export default {
    name:'headMenu',
    mounted() {
        this.$nextTick(function(){
            $('#channel-nev').lavalamp({
                easing:'easeOutBack'
            });
            window.addEventListener("scroll",this.onScroll);
        })
    },
    methods: {
        onScroll(){
            var top = $(document).scrollTop();
            if(top >= 140){
                $('.headMenu').addClass('menu-fix-top');

            }else{
                $('.headMenu').removeClass('menu-fix-top')
            }
        }
    }
}
</script>



<style>
.headMenu{
    width: 100%;
    height: 40px;
    margin-top: 8px;
    background-color: #01204f;
}
.menu{
    width: 984px;
    height: 40px;
    margin: 0 182.5px;
    z-index: 100;
    /* background-color: #fff; */
}
.menu ul{
    width: 984px;
    height: 40px;
    margin: 0;
    padding: 0;
    list-style: none;
    display: block;
}
.menu-item{
    width: 48px;
    height: 40px;
    line-height: 40px;
    text-align: center;
    font-size: 16px;
    display:block;
    float: left;
    font-family: arial,"Hiragino Sans GB","Microsoft Yahei","微软雅黑","宋体",Tahoma,Arial,Helvetica,STHeiti;
}
.menu-index{
    width: 68px;
    height: 40px; 
}
.menu-index a{
    padding-left: 24px;
    background-image: url("../images/icon-index.png");
    background-repeat: no-repeat;
    background-position: 1px -3px;
}
.menu-item a{
    text-decoration: none;
    font-size: 14px;
    font-weight: 700;
    color: #fff;
}
.person{
    display: block;
    width: 76px;
    height: 40px;
    text-decoration: none;
    font-size: 14px;
    font-weight: 700;
    color: #fff;
}
.headMenu a:link,.headMenu a:visited,.headMenu a:hover{
    columns: #fff;
    text-decoration: none;
}
.headMenu .menu .current{
    background-color: #c00;
}
.lavalamp-object {
  background-color: #c00;
  transition-duration: 0.7s;
}


</style>


