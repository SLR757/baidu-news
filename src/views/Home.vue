<template>
    <div id="home">
      <div id="body">
        <FocusNews></FocusNews>
        <router-view></router-view>
    </div>
    </div>
</template>


<script>
// @ is an alias to /src
import FocusNews from "@/components/FocusNews.vue";

export default {
  name: "home",
  components: {
    // Head
    FocusNews
  }
};
</script>

<style scoped>
/* @import '../css/head.css'; */
</style>

