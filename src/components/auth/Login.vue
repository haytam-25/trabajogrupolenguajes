<script setup>
    import {ref} from 'vue';
    
    const sEmail=ref('');
    const sPassword=ref('');

    const sEmailre=ref('');
    const sPasswordre=ref('');
    const sRepetirPassword=ref('');

    function loginPresionado(){
        alert("El usuario escrito es "+sEmail.value+" y la contra escrita es  "+sPassword.value);

    }

    function registroPresionado(){

    }

    
    function registrarPresionado(){
        alert("El usuario escrito es "+sEmailre.value+" y la contra escrita es  "+sPasswordre.value);

    }

    function cancelarPresionado(){

    }

</script>

<template>
    <div class="contenedor">
        <div id="login">

            <h2>LOGIN</h2>

            <input  type="text" placeholder="Email o usuario" v-model="sEmail"/>
            <input  type="password" placeholder="Contraseña"v-model="sPassword"/>


            <button @click="loginPresionado">LOGIN</button>

            <button @click="registroPresionado">REGISTER</button>

        </div>
        
        <div id="register">
            <h2>Register</h2>

            
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

    #login{
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
