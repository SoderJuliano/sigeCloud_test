<template>
<div class="main-container" style="display:block">
    <Header />
    <Body 
        cor="#004798"
        fatura=true
        position="relative"
    />
    <div class="midle">
        <p>Compre agora com <span>10%</span> de desconto!</p>
    </div>
    <div class="item-midle">
        <img src="../assets/recorte-cart.png"  alt="carrinho" /><span >Itens no carrinho</span>
        <div v-for="item in products" :key="item"  class="itens">
            <div :style="[products.indexOf(item) % 2 === 0 ? {'background-color': '#F5F5F5'} : '' ]" class="row">
                <div style="display: flex; width:30%">
                    <div style="padding: 6px; background-color: #004798; border-radius: 2px">
                        <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 15 15"><path d="M19.5,17.833V6.167A1.672,1.672,0,0,0,17.833,4.5H6.167A1.672,1.672,0,0,0,4.5,6.167V17.833A1.672,1.672,0,0,0,6.167,19.5H17.833A1.672,1.672,0,0,0,19.5,17.833ZM9.083,13.25l2.083,2.508L14.083,12l3.75,5H6.167Z" transform="translate(-4.5 -4.5)" fill="#f5f5f5"/></svg>
                    </div>
                    <div class="item-name">
                        <p>{{item.name}}</p>
                        <a href="#">Ver anúncio</a>
                    </div>
                </div>
                <div class="value">
                    <span>De R$ {{item.value}} por</span>
                    <span style="font-size:15px; color:#72BF44; font-weight: bolder !important; float:right; margin-top: -2px">
                        {{item.newValue}}
                    </span>
                </div>
                
            </div>
        </div>
        
    </div>
    <BntMultiText />
    <ContatctContainer />
    <Footer />
</div>
</template>

<script>
import Header from './Header.vue'
import Body from './Body.vue'
import Footer from './Footer.vue'
import BntMultiText from './BntMultiText.vue'
import ContatctContainer from './ContactContainer.vue'

export default {
    name: 'dashboard',
    components: {
       Header,
       Body,
       Footer,
       BntMultiText,
       ContatctContainer
    } ,
    data(){
        return{
             products:[
                {
                    "name":"Chromecast",
                    "value":"219,90",
                    "newValue":"197,91"
                },
                {
                    "name":"JBL Flip 3",
                    "value":"339,50",
                    "newValue":"359,55"
                },
                {
                    "name":"Kindle Peperwhite",
                    "value":"319,90",
                    "newValue":"287,91"
                }
             ]
        }
    }   
}
</script>

<style scoped>
@media screen and (min-width: 701px) {
.main-container{
    max-width: 700px;
    width: 60%;
    border: 1px solid black;
    height: 100%;
    overflow: hidden;
    justify-content: space-around;
    text-align: center;
    margin: 0 auto;
}
}
p{
  color: #004798;
  font-weight: bolder;
  text-align: center;
  font: normal normal bold 12px Segoe UI;
}
p span{
    background-color: #BDECC4;
}
.midle{
    width: 100%;
    display: block;
    margin-top: 30px;
    align-content: center;
}
.item-midle{
    border: 1px solid #BDBDBD;
    width: 80%;
    margin: 0 auto;
    height: 30%;
    min-height: 130px;
    padding: 20px;
    padding-bottom: 0px;
    border-radius: 5px;
    margin-top: 25px;
    text-align: center;
    overflow: hidden;
}
.item-midle span{
    top: -9px;
    font: normal normal bold 12px Segoe UI;
    position: relative;
    font-weight: bolder;
}
.item-midle img{
    position: relative;
    left: -10px;
}
@media screen and (min-width: 701px) {
    .row{
        height: 28px;
        position: relative;
        width: 107%;
        left: -7%;
        padding: 10px;
        display: flex;
        justify-content: space-between;
        padding-left: 8%;
    }
    .row a{
        left: -30px;
    }
}
@media screen and (max-width: 700px) {
    .row{
        height: 28px;
        position: relative;
        width: 110%;
        left: -7%;
        padding: 10px;
        display: flex;
        justify-content: space-between;
        padding-left: 20px;
        padding-right: 20px;
    }
    .row a{
        left: -15px;
    }
}

.row p{
    font: normal normal bold 12px Segoe UI;
    color: #383434;
    font-weight: bolder;
    position: relative;
    top: 10px;
    min-width: 110px;
    text-align: start;
}
.row a{
    
    text-decoration:none;
    font: normal normal 300 10px Segoe UI;
    color: #757575;
    top: -9px;
    position: relative;
    text-align: left;
}
.item-name{
    justify-content: left;
    height: 30px;
    margin-top: -20px;
    margin-left: 10px;
    min-width: 80px;
    font-weight: 800;
}
.value{
    display: flex;
    position: relative;
    top: 15px;
    right: 25px;
}
.value span{
    font: normal normal 300 10px Segoe UI;
    color: #757575;
    margin-right: 10px;
    margin-top: 1px;
}
.itens{
    margin-top: 10px;
}
</style>