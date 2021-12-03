<template>
    <div>
       <v-card>
           <v-card-title >{{producto.nombre}}</v-card-title>
           <v-card-text>
               <p>Precio: $ {{producto.precio}}</p>
               <p v-if="producto.cantidad > 0">Cantidad: {{producto.cantidad}}</p>
               <v-chip v-else dark>Sin Stock</v-chip>
           </v-card-text>

           <v-card-text></v-card-text>
           
           
           
       </v-card>
    </div>
</template>

<script>
    export default {
        props:{
            producto:Object
        }
    }
</script>

<style lang="scss" scoped>

</style>