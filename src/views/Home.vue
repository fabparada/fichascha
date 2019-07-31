<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Galeria></Galeria>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Galeria from '@/components/Galeria.vue'

export default {
  name: 'home',
  components: {
    Galeria
  }
}
</script>
