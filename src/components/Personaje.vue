<template>
    <div class="personaje">
        <img src="../assets/goku.png">
        <p>Fuerza Actual: {{fuerzaActual}}</p>
        <button @click="cabrear">Cabrear a goku</button>
    </div>
</template>

<script>
import {ref} from 'vue'

export default {
    name:'Personaje',
    props:{
        fuerza:{
            type:Number,
            default: 0,
            required:true
        },
        imagen:{
            type:String,
            default: 'goku.png'
    
        }
    },

    setup(props){
        let fuerzaActual=ref(props.fuerza)
        let imagenDePersonaje=props.imagen

        const cabrear=()=>{
            console.log(fuerzaActual)
            fuerzaActual.value++
        }

        return {
            fuerzaActual,
            cabrear,
            imagen: imagenDePersonaje
        }
    }
}
</script>

<style lang="scss" scoped>

</style>