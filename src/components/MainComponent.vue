<template>
    
    <div >
        <img src="../assets/images/jumbotron.jpg"  class="jumbotron">
    </div>
    
  <section class="text-uppercase serie">
    <div class="container ">
            <button class="btn mt-3 ">Current series</button>
            <div class="row mt-3">
                <CardApp v-for="comic, index in comicsCard" :thumb="comic.thumb" :key="index" />
            </div>
            <div class="d-flex justify-content-center ">
                <button class="btn mb-3">Load more</button>
            </div>
        </div>
        </section>
         <IconsNav />
</template>

<script>
import IconsNav from './main/IconsNav.vue';
import CardApp from './main/CardApp.vue';
import { cardComics } from './main/dcComic.js'
    export default {
        name:'MainComponent',
        components: {
            IconsNav,
            CardApp
           
        },
        data(){
            return{
                comicsCard :cardComics
            }
        }
    }
</script>

<style lang="scss" scoped>
    main{
        background-color: black;
        color: white;
    }
    .serie{
        background-color: black;
    }
    
    h3{
        padding:20px;
    }
    .jumbotron{
        width: 100%;
        height: 400px;
        object-fit: cover;
        object-position: top;
    }
    .btn {
        background-color: blue;
        color: white;
        
        
    }

</style>