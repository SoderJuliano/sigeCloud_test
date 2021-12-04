<template>
    <button>Ir para área de pagamento</button>
    
</template>
<script>
export default {
    name: 'bnt-payment',
}
</script>
<style scoped>
button{
    max-width: 200px;
    width: 45%;
    height: 45px;
    background-color: #00C853;
    padding: 10px;
    border-radius: 5px;
    border: none;
    font-family: 'Segoe';
    font-weight: bolder;
    color: white;
}
@media screen and (min-width: 701px) {
 button{
    font-size: 14px;
 }   
}

@media screen and (max-width: 701px) {
  button{
    font-size: 12px;
 }  
}
</style>