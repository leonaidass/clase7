<template>
    <div>
         <h2>Listado de Productos</h2>

         <v-row>
             <v-col v-for="(producto,i) in productos" :key="i">
               
                 <Cardproducto
                 :producto="producto"
                 />  

             </v-col>
         </v-row>
    </div>
</template>

<script>

    import Cardproducto from "./Cardproducto.vue"
    export default {

        props:{
            productos:Array
        },
        components:{
            Cardproducto
        }
        
    }
</script>

<style lang="scss" scoped>

</style>