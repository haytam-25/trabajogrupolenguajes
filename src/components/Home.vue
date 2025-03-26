<script setup>
    import {defineProps} from 'vue';
    import Login from './auth/Login.vue';
    import Register from './auth/Register.vue';


    const props = defineProps({
        sTitulo:{
            type: String,
            default: 'TITULO APP'
        }
    });

    function MostrarRegistro(){
        alert("HEMOS LLEGADO A MOSTRAR REGISTRO LOCO");
    }


</script>

<template>
    <div class="contenedor">
            
            <h1> {{sTitulo}} </h1>
            <img src="../assets/descarga.jpg" alt="raphi" class="LOGO"/>
        
        <div class="loginregister">
            
            <Login v-if="true" @cambioARegistro="MostrarRegistro"></Login>
            <Register v-if="false"></Register>
        
        </div>
    </div>
</template>

<style scoped>

.contenedor{
    display: flex;
    flex-direction: column;
    align-items: center;
    }
    
.LOGO{
    height: auto;
    width: auto;
}
</style>
