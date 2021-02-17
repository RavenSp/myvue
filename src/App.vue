<template>
  <div id="app">
      <Top />
      <Nav />
      <div class="main-content">
        <div class="container-fluid" style="text-align: justify;">
          <div class="row">
            <div class="col">
              {{ test }}
          </div>
          </div>
         
        
        </div>
        
      </div>
    <router-view/>
     </div>
</template>

<style>
  @import 'https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/css/bootstrap.min.css';
  @import 'https://use.fontawesome.com/releases/v5.0.13/css/all.css';
  :root {
    --main-color: rgb(47, 127, 38);
  };

  body,
  html {
    margin: 0;
    padding: 0;
  }

  .main-content {
    margin-top: 50px;
    margin-left: 50px;
    margin-right: 0px;
    margin-bottom: 0px;
  }

  .v-sidebar-menu .vsm--item .vsm--link_level-1.vsm--link_active {
    box-shadow: 3px 0px 0px 0px var(--main-color) inset;
    }

  .v-sidebar-menu .vsm--link_level-1:hover .vsm--icon {
    background-color: var(--main-color);
  }

  .v-sidebar-menu.vsm_collapsed .vsm--mobile-bg  {
    background-color: var(--main-color);
  }

  .v-sidebar-menu.vsm_collapsed .vsm--link_level-1:hover .vsm--icon, .v-sidebar-menu.vsm_collapsed .vsm--link_mobile-active:hover .vsm--icon  {
    background-color: white !important;
    color:  var(--main-color) !important;
  }



</style>

<script>

  import Nav from "./components/Nav"
  import Top from "./components/Top"
 
 export default {
  components: {Nav, Top},

  data() {
    return {
      test:'message'
    }
  }
 }




</script>