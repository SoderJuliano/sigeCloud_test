<template>
<div>
    <Header />
    <Body />
</div>
</template>

<script>
import Header from './Header.vue'
import Body from './Body.vue'

export default {
    name: 'dashboard',
    components: {
       Header,
       Body
    }    
}
</script>