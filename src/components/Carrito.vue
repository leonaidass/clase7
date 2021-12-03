<template>
    <v-data-table
    :headers="carritoheaders"
    :items="desserts"
    class="elevation-1"
    hide-default-footer
  ></v-data-table>
</template>

<script>
    export default {
        props:{
            productosCarrito:Array
        },
        data() {
            return {
                carritoheaders:[
          { text: 'Nombre de Prducto', value: 'nombre' },
          { text: 'Precio', value: 'precio' },
          { text: 'Cantidad', value: 'cantidad' },
          
        ]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>