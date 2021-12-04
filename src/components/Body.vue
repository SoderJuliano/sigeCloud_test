<template>
    <div :style="`background-color:${cor}; position:${position}`"  class="main">
        <div v-if="`${fatura}`" class="fatura">
            <Item
                class="item"
                :title=title
                :texto1=plano50Mb
                :texto3=Mb50R$
                texto4="Seguro Saúde Carlos And(...)"
                :texto5=parcelaSeguro
                :texto52=totaisDeParcelasSeguro
                texto6="R$ 49,90"
                texto7="Roteador TP-Link Archer(...)"
                :texto8=parcelaRoteador
                :texto82=totaisDeParcelasTP
                texto9="R$ 26,55"
                texto10="Valor total da fatura"
                texto11=""
                texto12="R$ 166,25"
            />
        </div>
        <div style="padding: 20px; width:100%; margin-left: 20%;" class="payment">
            <BntPayment class="payment-bnt"/>
        </div>
    </div>
</template>
<script>
import Item from './Item.vue'
import BntPayment from './BntPayment.vue'

export default {
    name: 'body',
    components:{
        Item,
        BntPayment
    },
    data(){
        return{
            title: "Item da fatura",
            plano50Mb: "Plano Internet 50MB",
            Mb50R$: "R$ 89,80",
            parcelaSeguro:3,
            totaisDeParcelasSeguro:6,
            parcelaRoteador:5,
            totaisDeParcelasTP:6
        }
    },
    props:{
        cor:String,
        fatura:Boolean,
        position:String
    }
}
</script>
<style scoped>
.fatura{
    display: block;
    padding-top: 10px;
}
.main{
    min-height: 300px;
    justify-content: center;
}
.item{
    margin-top: 20px;
}
@media screen and (max-width: 700px) {
    .main{
        width: 100vw;
        height: 35%;
        margin-left: -8px;
    }
}
@media screen and (min-width: 701px) {
    .main{
        width: 400px;
    }
}

</style>