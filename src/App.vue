<template>
  <div id="app">
    <Head></Head>
  
    <router-view/>
      <Footer></Footer>
  </div>
</template>


<script>
import Head from './components/Head/Head.vue'
import Footer from './components/Footer/Footer.vue'

export default {
  name:'App',
  components: {
    Head,
    Footer
  }
}
</script>



<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body{
  margin:0;
  padding: 0;
}

// 全局清除浮动
.clearfix:after {
    clear: both;
    content: '.';
    display: block;
    font-size: 0;
    line-height: 0;
    visibility: hidden;
    height: 0
}

ul{
  list-style: none;
  margin: 0;
  padding:0;

}
a{
  text-decoration: none;
}
</style>
