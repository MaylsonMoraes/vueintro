<template>
    <form action="" @submit="enviarFormulario($event)">
        <h2>Meu formulário:</h2>
        <div>
        <input type="text" v-model="name">
        </div>
        <div>
        <input type="text" v-model="email">
        </div>
        <div>
        <Customsubmit /> 
        </div>
    </form>
    <p>Conteúdo</p>
    <p>Conteúdo</p>
    <p>Conteúdo</p>
</template>
<script>
import inputText from './Form/inputText'
import Customsubmit from './Form/submit'

export default {
    name:'Customform',
    components: {
        inputText,
        Customsubmit
    },
    data() {
        return {
            name:"",
            email:""
        }
    },
    methods: {
        enviarFormulario(e) {
            e.preventDefault();
            const name = this.name;
            const email = this.email;

        console.log("formulario enviado!");
        console.log("O nome é:"+ name);
        console.log("O email é:"+ email);
        
        // ajax
        // inserir no banco de dados

        }
    }
}
</script>

<style scoped>
p {
    margin: 150px;
}
</style>
