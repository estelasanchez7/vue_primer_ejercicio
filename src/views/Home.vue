<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  
    <Imagen/>
    <Imagen/>
   
  
  </div>
</template>

<script>
// @ is an alias to /src

import Imagen from '@/components/Imagen.vue'


export default {
  name: 'Home',
  components: {
    Imagen
  }
}
</script>
