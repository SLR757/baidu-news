<template>
    <div id="FocusNews">
        <FocusNewsLeft></FocusNewsLeft>
        <FocusNewsRight></FocusNewsRight>
        <router-view></router-view>
    </div>
</template>

<script>
import FocusNewsLeft from "@/components/FocusNewsLeft.vue";
import FocusNewsRight from "@/components/FocusNewsRight.vue";

export default {
  name: "FocusNews",
  components: {
    FocusNewsLeft,
    FocusNewsRight
  }
};
</script>

<style scoped>
#FocusNews{
  width: 984px;
  height: 1169px;
  margin: 0 auto;
  background-color: azure;
  margin-top: 12px;
  margin-bottom: 31px;
}
</style>


