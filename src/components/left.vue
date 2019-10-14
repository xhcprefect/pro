<template>
<div class="left">
    <h1>left</h1>
<!-- <v-news v-for=""></v-news> -->
      <v-news v-for="item in news" :aa='item' :key="item.id"></v-news>
</div>
</template>
<script>
import vNews from './news';
export default {
    data(){
        return{
            news:[
                {   
                    id:1,
                    title:'新闻一',
                    content:'韩国女星自杀',
                    time:1571051223584,
                },
                 {   
                    id:2,
                    title:'新闻二',
                    content:'韩国女星自杀',
                    time:1571051223584,
                },
                 {   
                    id:3,
                    title:'新闻三',
                    content:'韩国女星自杀',
                    time:1571051223584,
                },
                 {   
                    id:4,
                    title:'新闻四',
                    content:'韩国女星自杀',
                    time:1571051223584,
                },
            ]
        }
    },
    
    components: {
        vNews,   
    }
}
</script>
<style>
.left{
    width: 400px;
    background-color: purple;
}
</style>