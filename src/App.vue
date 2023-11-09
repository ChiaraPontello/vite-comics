<template>
  <HeaderComponent />
 
 <MainComponent />

<FooterApp />
</template>



<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import FooterApp from './components/FooterApp.vue'
  export default {
    name:'App',
    components: {
      HeaderComponent,
      MainComponent,
      FooterApp
    },
    data(){
      return{

      }
    },
    methods:{

    }
  }
</script>

<style lang="scss" scoped>

</style>
