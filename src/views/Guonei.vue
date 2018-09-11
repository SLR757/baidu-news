<template>
    <div id="guonei">
        <Head/>
    <router-view></router-view>
    </div>
</template>

<script>
import Head from '@/components/Head.vue'

export default {
    name:'guonei',
    components:{
        Head
    }
}
</script>

