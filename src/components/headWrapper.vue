<template>
    <div class="headWrapper">
        <div class="headSerach">
            <div class="box">
                <div class="logo">
                    <a href="#" id="logo"><img src="../images/logo_news.png" alt=""></a>
                </div>
                <table class="serach-box">
                   <tr>
                       <td id="inb">
                           <span><input type="text"></span>
                            <div class="btn"><button>百度一下</button></div>
                       </td>
                       <td id="help">
                            <div class="rowa">
                                <a href="#">帮助</a>
                                <a href="#">高级搜索</a>
                                <a href="#">设置</a>
                            </div>
                           
                       </td>
                   </tr>
                   <tr>
                       <div id="sel">
                            <input type="radio" name="radios" value="1" v-model="param"><label>新闻全文</label>
                            <input type="radio" name="radios" value="2" v-model="param"><label>新闻标题</label>

                       </div>
                   </tr>
                </table>
            </div>
        </div>
       
    </div>
</template>

<script>
export default {
  name: "headWrapper",
  data(){
        return{
            param:'1' //设置默认值为1，即设置第一个单选框为选中状态
        }
    }
};
   
</script>

<style scoped>
.headWrapper {
  padding-top: 31px;
  width: 100%;
  height: 65px;
  /* background-color: rgb(205, 219, 219); */
}
.headSerach {
  width: 995px;
  height: 65px;
  margin: 0 auto;
  background-color: #fff;
}
.box {
  width: 940px;
  height: 65px;
  margin-left: 87px;
  margin-bottom: 7px;
}
#logo {
  display: inline-block;
  width: 155px;
  height: 50px;
  float: left;
  position: relative;
  top: -10px;
  /* background-image: url(../images/logo_news.png) */
}
#logo img {
  width: 135px;
  height: 45px;
  float: left;
}
.serach-box {
  display: inline-block;
  width: 785px;
  height: 66px;
  float: left;
}

#inb {
  width: 616px;
  height: 40px;
  padding: 0;
}
span {
  display: inline-block;
  width: 510px;
  height: 40px;
  border: 1px solid #ebebeb;
  float: left;
}
span input {
  font-size: 16px;
  width: 502px;
  height: 25px;
  margin-left: 8px;
  margin-top: 5px;
  border: none;
  border-collapse: collapse;
  outline: 0;
}
.btn {
  display: inline-block;
  background-color: #38f;
  width: 104px;
  height: 42px;
}
.btn button {
  width: 100%;
  height: 40px;
  background-color: #38f;
  border-collapse: collapse;
  background-color: none;
  border: 1px solid #38f;
  color: #fff;
  font-size: 16px;
  cursor: pointer;
}
#help {
  width: 147px;
  height: 40px;
  padding: 0;
  
}
.rowa {
  width: 100%;
  height: 18px;
  line-height: 40px;
  text-align: center;
  display: flex;
  justify-content: space-around;
}
#help a {
  height: 15px;
  line-height: 15px;
  text-align: center;
  font-size: 13px;
  color: #2c3e50;
  vertical-align: middle;
}
#sel{
    width: 200px;
    height: 18px;
    margin-top: 5px;
    font-size: 12px;
    float: left;
}
#sel input,label{
    float: left;
}
#sel label{
    margin-right: 15px;
}



</style>



