<template>
<div class="main">
    <v-left></v-left>
    <v-right></v-right>
</div>
</template>
<script>
import vLeft from './left';
import vRight from './right'
export default {
    components:{
        vLeft,
        vRight
    }
}
</script>
<style>
.main{
    flex: 1;
    background-color: skyblue;
    display: flex;
}
</style>