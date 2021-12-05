<template>
    <div class="footer">
        <img src="../assets/logo-sigecloud.svg" alt="">
    </div>
</template>

<style scoped>


@media screen and (min-width: 701px) {
    img{
        margin: 0 auto;
        width: 15%;
        max-width: 160px;
        margin-bottom: 10px;
    }
    .footer{
        display: flex;
        justify-content: center;
        background-color: white;
        bottom: 0px;
        left: 0;
        height: 7%;
        width: 100%;
        min-height: 40px;

    }
}
@media screen and (max-width: 701px) {
    img{
        margin: 0 auto;
        width: 35%;
    }
    .footer{
        display: flex;
        justify-content: center;
        background-color: white;
        position: fixed;
        bottom: 0px;
        left: 0;
        height: 7%;
        width: calc(100vw + 5px);
        min-height: 40px;

    }
}
</style>