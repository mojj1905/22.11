<template>
  <div class="container">
    <h1 class="text-center mt-3">Body</h1>
    <div class="row">
      <div class="col-4" v-for="item in 3" :key="item">
        <div class="card my-3" style="width: 18rem">
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
            <p class="card-text">
              {{star.description}}
              
            </p>
            <a href="#" class="card-link">Card link</a>
            <a href="#" class="card-link">Another link</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
        star : {}
        
    }
    console.log(star);
  },
  props : {
    producs : {
        type : Array
    }
  },
  
}
</script>

<style scoped>
</style>