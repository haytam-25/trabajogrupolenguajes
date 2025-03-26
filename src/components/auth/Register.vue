<script setup>
    import {ref} from 'vue';
    
   

    const sEmailre=ref('');
    const sPasswordre=ref('');
    const sRepetirPassword=ref('');



    function registrarPresionado(){
        alert("El usuario escrito es "+sEmailre.value+" y la contra escrita es  "+sPasswordre.value);

    }

    function cancelarPresionado(){
        blLoginVisible.value=true;
        blRegisterVisible.value=false;

    }

</script>

<template>
    <div class="contenedor">
        
        
        <div id="register">
            <h2>Registro</h2>

            
            <input  type="text" placeholder="Email o usuario" v-model="sEmailre"/>
            <input  type="password" placeholder="Contraseña"v-model="sPasswordre"/>
            <input  type="password" placeholder="Repetir Contraseña"v-model="sRepetirPassword"/>


            <button @click="registrarPresionado">REGISTRAR</button>

            <button @click="cancelarPresionado">CANCELAR</button>

            
        </div>

    </div>



</template>

<style scoped>
    .contenedor {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 300px;
    }

    

    #register{
        margin-top: 30px;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 300px;
    }
    




</style>
