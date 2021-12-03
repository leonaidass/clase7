<template>
     <v-card class="pa-4">
         <h3>{{titulo}}</h3>
         <v-btn @click="eventoPersonalizado">
             Enviar
         </v-btn>
       </v-card>
</template>

<script>
    export default {

        props:{
            titulo:String
        },
        data() {
            return {
                mensaje: " mensaje desde sidebar"
            }
        },
        methods:{
            eventoPersonalizado(){
                this.$emit("eventoNuevo",this.mensaje)
                console.log("entral al metodo")
                 
            }
        }
        
    }
</script>

<style lang="scss" scoped>

</style>