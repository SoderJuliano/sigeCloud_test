<template>
<div class="main-item">
    <div class="header">
        <span>{{title}}</span>
        <span style="float:right">valor</span>
    </div>
    <div class="body">
        <div class="line">
            <span v-if="texto1">{{texto1}}</span>
            <span style="font-size:11px; color:#383434" v-if="texto2">{{texto2}}</span>
            <span style="color:#72BF44; font-weigth:bolder; float:right" v-if="texto3">{{texto3}}</span>
        </div>
        <div class="line">
             <span v-if="texto4">{{texto4}}</span>
            <span style="font-size:11px; color:#383434" v-if="texto5">({{texto5}} de {{texto52}})</span>
            <span style="color:#72BF44; font-weigth:bolder; float:right" v-if="texto6">{{texto6}}</span>
        
        </div>
        <div class="line">
             <span v-if="texto7">{{texto7}}</span>
            <span style="font-size:11px; color:#383434" v-if="texto8">({{texto8}} de {{texto82}})</span>
            <span style="color:#72BF44; font-weigth:bolder; float:right" v-if="texto9">{{texto9}}</span>
        
        </div>
    </div>
    <div class="footer">
         <span v-if="texto10">{{texto10}}</span>
        <span v-if="texto11">{{texto11}}</span>
        <span style="font-size:15px; color:#72BF44; font-weigth:bolder; float:right" v-if="texto12">{{texto12}}</span>
    </div>
</div>
    
</template>

<script>
export default {
    name: 'item',
    props:{
        title: String,
        texto1: String,
        texto2: String,
        texto3: String,
        texto4: String,
        texto5: Number,
        texto52: Number,
        texto6: String,
        texto7: String,
        texto8: Number,
        texto82: Number,
        texto9: String,
        texto10: String,
        texto11: String,
        texto12: String,
    }
}
</script>

<style scoped>
.main-item{
    background-color: white  !important;;
    width: 75%;
    min-height: 130px;
    padding: 20px;
    margin: 0 auto;
    margin-top: 20px;
    border-radius: 5px;
}
.line{
    margin-top: 11px;
    width: 100%;
    font: normal normal bold 12px Segoe UI;
}
.header{
    justify-content: space-between;
    font: normal normal 300 12px Segoe UI;
    color: #9E9E9E;
    position: relative;
    margin-top: -10px;
}
.body{
    margin-top: 20px;
}
.footer{
    margin-top: 30px;
    font: normal normal bold 12px Segoe UI;
    letter-spacing: 0px;
}
</style>