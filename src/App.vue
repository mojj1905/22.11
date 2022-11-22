<script setup>
import HeaderVue from './components/Header.vue';
import axios from 'axios'
import BodyVue from './components/Body.vue';
</script>
<template>
  <div>
    <HeaderVue/>
    <BodyVue :producs="producs"/>
  </div>
</template>

<script>
export default {
  data() {
    return{
      producs : []
    }
  },
  created(){
    this.axios.get('https://fakestoreapi.com/products?limit=3').then(({data})=>{
      this.producs=data
     

    })
  }
}
</script>

<style scoped>

</style>