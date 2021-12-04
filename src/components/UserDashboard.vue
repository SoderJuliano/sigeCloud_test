<template>
<div style="display:block">
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
        <div style="background-color: #F5F5F5" class="row">

        </div>
        <div class="row">
            
        </div>
        <div style="background-color: #F5F5F5" class="row">
            
        </div>
    </div>
    <Footer />
</div>
</template>

<script>
import Header from './Header.vue'
import Body from './Body.vue'
import Footer from './Footer.vue'

export default {
    name: 'dashboard',
    components: {
       Header,
       Body,
       Footer,
    }    
}
</script>

<style scoped>
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
    margin-top: 20px;
    align-content: center;
}
.item-midle{
    border: 1px solid #BDBDBD;
    width: 75%;
    margin: 0 auto;
    height: 30%;
    min-height: 130px;
    padding: 20px;
    border-radius: 5px;
    margin-top: 25px;
    text-align: center;
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
.row{
    height: 40px;
    position: relative;
    width: 114%;
    left: -7%;
}
</style>