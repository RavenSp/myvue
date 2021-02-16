<template>
  <div id="app">
    <div class="container">
    <h1>Test App</h1>
    
  </div>  
  
    <router-view/>
   <Nav />
  </div>
</template>

<style>
  @import 'https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/css/bootstrap.min.css';
  @import 'https://use.fontawesome.com/releases/v5.0.13/css/all.css';

</style>

<script>

  import Nav from "./components/Nav"
 
 export default {
  components: {Nav}
 }




</script>