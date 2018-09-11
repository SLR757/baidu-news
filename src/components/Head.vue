<template>
  <div class="head">
    <headTop></headTop>

    <headWrapper></headWrapper>
    <headMenu></headMenu>
    
  </div>
</template>

<script>
  import headTop from "@/components/headTop.vue";
  import headWrapper from "@/components/headWrapper.vue";
  import headMenu from "@/components/headMenu.vue";

  export default {
    name: "Head",
    props: {
      msg: String
    },
    components: {
      headTop,
      headWrapper,
      headMenu
    }
  };
</script>



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
