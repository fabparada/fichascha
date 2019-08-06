<template>
<div class="container-fluid bg-blue">
  <div class="container">
    <img class="d-block ml-3" src="../assets/gob.svg" width="105" alt="">

    <nav class="navbar pt-0 navbar-expand-lg navbar-light bg-blue">
    <!-- <a class="navbar-brand text-white" href="#">
      <img src="../assets/by.svg" alt=""> 
    </a> -->
    
    <a class="" href="http://" target="_blank" rel="noopener noreferrer">
    
      <!-- <img class="d-block " src="../assets/gob.svg" width="105" alt=""> -->
      <img class="d-block " src="../assets/by.svg" width="105" alt="">
    </a>
     

    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto">
       
        <li class="nav-item">
          <a class="nav-link text-white my-4 py-0 my-2 border-right" href="#">¿Qué es chileatiende?</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link my-4 py-0 dropdown-toggle text-white" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Contáctenos
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item text-white" href="#">Action</a>
            <a class="dropdown-item text-white" href="#">Another action</a>
            <div class="dropdown-divider"></div>
            <a class="dropdown-item text-white" href="#">Something else here</a>
          </div>
        </li>
      
      </ul>

      <form class="form-inline my-2 my-lg-0">
        <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
          <i class="material-icons">
            search
          </i>
        </button>
      </form>
    </div>
  </nav> 
  </div>
</div>
</template>

<script>
  export default{
    data () {
      return {
        brand: 'cirso de vue.js'
      }
    }
  }
</script>
<style>
  .bg-blue{
    background-color: #072651;
  }
 
</style>