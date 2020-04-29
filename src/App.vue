<template>
  <div id="app">
    <div class="bg-danger">
      <h3 class="title">{{name}}</h3>
    </div>
    <gallery />
  </div>
</template>

<script>
  import Gallery from './components/Gallery.vue'

  export default {
    name: 'App',
    components: { Gallery },
    data(){
      return {
        name: 'Book Gallery',
      }
    }
  }
  
</script>

<style>
  .title {
    text-align: center;
  }
  html {
    font-size: 1rem;
  }
</style>
