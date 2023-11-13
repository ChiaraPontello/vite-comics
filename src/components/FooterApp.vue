<template>
    <footer>
        <FooterUp />
        <FooterDown />
    </footer>
</template>

<script>
import FooterUp from './footer/FooterUp.vue';
import FooterDown from './footer/FooterDown.vue'
    export default {
        name:'FooterApp',
        components:{
            FooterUp,
            FooterDown
            
        }
    }
</script>

<style lang="scss" scoped>

</style>