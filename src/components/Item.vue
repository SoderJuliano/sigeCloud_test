<template>
<div class="main-item">
    <div class="header">
        <span style="float: left">{{title}}</span>
        <span style="float:right">Valor</span>
    </div>
    <div class="body">
        <div class="line">
            <span v-if="texto1">{{texto1}}</span>
            <span  style="font: normal normal 300 10px Segoe UI; font-weight: 300; opacity: 80%" v-if="texto2"> (Parcela{{texto2}})</span>
            <span style="color:#72BF44; font-weigth:bolder; float:right" v-if="texto3">{{texto3}}</span>
        </div>
        <div class="line">
             <span v-if="texto4">{{texto4}}</span>
            <span  style="font: normal normal 300 10px Segoe UI; font-weight: 300; opacity: 80%" v-if="texto5"> (Parcela{{texto5}} de {{texto52}})</span>
            <span style="color:#72BF44; font-weigth:bolder; float:right" v-if="texto6">{{texto6}}</span>
        
        </div>
        <div class="line">
             <span v-if="texto7">{{texto7}}</span>
            <span  style="font: normal normal 300 10px Segoe UI; font-weight: 300; opacity: 80%" v-if="texto8"> (Parcela{{texto8}} de {{texto82}})</span>
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
    width: 80%;
    min-height: 130px;
    padding: 25px;
    margin: 0 auto;
    margin-top: 20px;
    border-radius: 5px;
}
.line{
    margin-top: 15px;
    width: 100%;
    font: normal normal bold 12px Segoe UI;
    font-weight: 800;
    color: #383434;
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
@media screen and (max-width: 700px) {
    .main-item{
        font-size: 12px;
    }
}
@media screen and (min-width: 701px) {
     .main-item{
        font-size: 14px !important;
    }
    .body{
        justify-content: start;
        text-align: left;
        margin-top: 50px;
    }
    .footer{
        text-align: start;
    }
}
</style>