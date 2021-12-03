<template>
 <v-app>
   <Navbar/>

   <v-row class="mt-14">
     
     <v-col cols="3" >
        <Sidebar 
        titulo="Agregar Producto"
        @eventoNuevo="funcionMaestra($event)"
        />

      <!-- <Carrito/> -->
     </v-col>
     
     <v-col>
         
         <Cardcontainer
           :productos="productos"
         />

     </v-col>

   </v-row>
 </v-app>

   
</template>

<script>

import Navbar from "./components/Navbar.vue"
import Sidebar from "./components/Sidebar.vue"
import Cardcontainer from "./components/Cardcontainer.vue"
import productos from "./assets/data/productos.json"
// import Carrito from "./components/Carrito.vue"
  export default {
     components:{
            Navbar,
            Sidebar,
            Cardcontainer,
            // Carrito
        },
        data() {
          return {
           productos
          }
        },

        methods:{
          funcionMaestra(parametro){
            console.log("entra al metodo desde maestra",parametro)
          }
        }
  }
</script>

<style lang="scss" scoped>

</style>