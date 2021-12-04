<template>
    <div class="main">
        <span style="color: #383434; font: normal normal 300 12px Segoe UI;">Atenciosamente,</span><br>
        <span style="font: normal normal bold 12px Segoe UI;">Juliano Soder</span>
        <div class="whats">
            <a style="text-decoration: none; color: #383434" href="https://clicano.link/WhatsAppJulianoSoder">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20"><path d="M17,5.156a9.914,9.914,0,0,0-15.6,11.96L0,22.25l5.254-1.379a9.881,9.881,0,0,0,4.737,1.205h0a10.006,10.006,0,0,0,10-9.911,9.95,9.95,0,0,0-3-7.009ZM10,20.406a8.223,8.223,0,0,1-4.2-1.147l-.3-.179L2.384,19.9l.83-3.04-.2-.312a8.253,8.253,0,1,1,15.308-4.379A8.329,8.329,0,0,1,10,20.406Zm4.518-6.17c-.246-.125-1.464-.723-1.692-.8s-.393-.125-.558.125-.638.8-.786.973-.29.188-.536.063a6.741,6.741,0,0,1-3.371-2.946c-.254-.437.254-.406.728-1.353a.459.459,0,0,0-.022-.433c-.062-.125-.558-1.344-.763-1.839s-.406-.415-.558-.424-.308-.009-.473-.009a.917.917,0,0,0-.661.308,2.783,2.783,0,0,0-.866,2.067,4.851,4.851,0,0,0,1.009,2.563A11.066,11.066,0,0,0,10.2,16.268a4.846,4.846,0,0,0,2.973.621,2.536,2.536,0,0,0,1.67-1.179,2.071,2.071,0,0,0,.143-1.179C14.924,14.42,14.759,14.357,14.513,14.237Z" transform="translate(0 -2.25)" fill="#2cc3ff"/></svg>
                (51) 9 97415104
            </a>
        </div>
        <div @click="openEmail()" class="email">
            <svg xmlns="http://www.w3.org/2000/svg" width="20.785" height="16.4" viewBox="0 0 20.785 16.4"><g transform="translate(-1.607 -5)"><path d="M4.8,6H19.2A1.805,1.805,0,0,1,21,7.8V18.6a1.805,1.805,0,0,1-1.8,1.8H4.8A1.805,1.805,0,0,1,3,18.6V7.8A1.805,1.805,0,0,1,4.8,6Z" fill="none" stroke="#2cc3ff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/><path d="M21,9l-9,6.3L3,9" transform="translate(0 -1.2)" fill="none" stroke="#2cc3ff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/></g></svg>
            julianosoder1989@gmail.com
        </div>
    </div>
</template>

<script>
export default {
    name: 'contato',
    methods:{
        openEmail(){
            window.open('mailto:julianosoder1989@gmail.com?subject=Contato referente à&body=Estou entrando em contato referente...');
        }
    }
}
</script>

<style scoped>

@media screen and (min-width: 701px) {
    .main{
        background-color: #EEEEEE; 
        padding: 30px;
        height: 130px; 
        margin-top: 20px;
        width: 100%;
        position: relative;
        left: -10px;
        top: -10px;
        font: normal normal 300 14px Segoe UI;
        text-align: start;
    }
    .main span{
        margin-left: 20px;
    }
    .whats{
        margin-top: 10px;
        margin-left: 20px;
        font: normal normal 14px Segoe UI;
        color:#383434;
    }
    .email{
        margin-top: 5px;
        font: normal normal 14px Segoe UI;
        color: #383434;
        margin-left: 20px;
    }
}
@media screen and (max-width: 701px) {
    .main{
        background-color: #EEEEEE; 
        padding: 30px;
        height: 130px; 
        margin-top: 30px;
        width: 100vw;
        position: relative;
        left: -10px;
        font: normal normal 300 12px Segoe UI;
    }
    .whats{
        margin-top: 30px;
        font: normal normal 12px Segoe UI;
        color:#383434;
    }
    .email{
        margin-top: 10px;
        font: normal normal 12px Segoe UI;
        color: #383434;
    }
}

svg{
    position: relative;
    top: 5px;
    margin-right: 10px;
}
</style>