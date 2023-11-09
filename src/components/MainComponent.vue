<template>
    <main>
        <h3 class="container">
        Content goes here
        </h3>
     <IconsNav />   
    </main>
    
</template>

<script>
import IconsNav from './main/IconsNav.vue';
    export default {
        name:'MainComponent',
        components: {
            IconsNav
        }
    }
</script>

<style lang="scss" scoped>
    main{
        background-color: black;
        color: white;
    }
    h3{
        padding:20px;
    }


</style>