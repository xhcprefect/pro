<template>
<div class="news">
    <h1>{{aa.title}}</h1>
    <p>{{aa.content}}</p>
    <p>{{aa.time|timeFilter}}</p>
</div>
</template>
<script>
export default {
    props:['aa'],
    filters: {
        timeFilter(obj){
            var d=new Date(obj);
            var y=d.getFullYear();
            var m=(d.getMonth()+1).toString().padStart(2,'0');
            var day=d.getDay().toString().padStart(2,'0');
            return `${y}-${m}-${day}`;
        }
    },
}
</script>
<style >
.news{
    width: 80%;
    background: #ccc;
    border-radius: 10px;
    margin: 20px auto 0;
    padding-left: 20px;
}
</style>