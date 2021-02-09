<template>
  <div class="about">
    <h1>This is an about page</h1>
     <Imagen/>
    <Imagen/>
     <Imagen/>
  </div>
</template>

<script>
// @ is an alias to /src

import Imagen from '@/components/Imagen.vue'

export default {
  name: 'About',
  components: {
    Imagen
  }
}
</script>
