<template>
    <div class="header">
        <img src="../assets/logo-sigecloud.svg" alt="logo" />
        <BntPayment />
    </div>
</template>

<script>

import BntPayment from '@/components/BntPayment.vue'
export default {
    name: 'header',
    components:{
        BntPayment
    }
}
</script>

<style scoped>
@media screen and (max-width: 700px) {
.header{
    display: flex;
    width: 100%;
    height: 60px;
    justify-content: space-around;
    padding-top: 5px;
}   
.header img{
    width: 37%;
    margin-top: -5px;
}

}
</style>