<template>
    <div id="headTop" class="clearfix">
        <div class="top-left">
            <ul>
                <li><a href="#">百度首页</a></li>
                <li><a href="#">登录</a></li>
                <li><a href="#">注册</a></li>
                <li><a href="#">百度新闻客户端</a></li>

            </ul>
        </div>
        <div class="top-right">
            <ul>
                <li><a href="#" class="right-a">网页</a></li>
                <li><a href="#" class="right-a-news">新闻</a></li>
                <li><a href="#" class="right-a">贴吧</a></li>
                <li><a href="#" class="right-a">知道</a></li>
                <li><a href="#" class="right-a">音乐</a></li>
                <li><a href="#" class="right-a">图片</a></li>
                <li><a href="#" class="right-a">视频</a></li>
                <li><a href="#" class="right-a">地图</a></li>
                <li><a href="#" class="right-a">文库</a></li>
                <div class="line">|</div>
            </ul>
            
        </div>
    </div>
</template>

<script>
export default {
  name: "headTop"
};
</script>



<style scoped>
#headTop{
    border-bottom: 1px solid #ebebeb;
}
#headTop {
  width: 100%;
  height: 33px;
  /* background-color: #ccc; */
}
.top-left{
    height: 31px;
    line-height: 31px;
    text-align: center;
    float: right;
    
}
ul{
    margin: 0;
    padding-left: 0px;
}
ul li{
    margin: 0;
    padding: 0;
    list-style-type: none;
    display: inline;
}
a{
    text-decoration: underline;
    color: black;
    font-size: 13px;
    height: 31px;
    line-height: 31px;
    text-align: center;
    margin-right: 12px;
    margin-left: 12px;
    font-weight: 200;
}
.top-right{
    float: right;
}
.right-a{
    font-size: 13px;
    font-weight: 700;
    color: #333;
    font-family: Arial;
}
.right-a-news{
    font-size: 13px;
    font-weight: 700;
    color: #333;
    font-family: Arial;
    text-decoration: none;
}
.line{
    display: inline-block;
    font-weight: 100;
    font-size: 12px;
    margin-right: 10px;
    padding-left: 10px;
}
</style>

