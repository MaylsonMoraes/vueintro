<template>
<div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades!</p>
    <p>Utilizo as seguintes tecnologias</p>
    <ul>
        <li>Javascipt</li>
        <li>PHP</li>
        <li>Python</li>
    </ul>
    <p v-show="mostrar_email">Mande uma mensagem para:{{email}}</p>
    <p>Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">Basta clicar aqui</a></p>
    <Picture />
</div>
</template>
<script>
import Picture from './Form/Picture.vue'
export default {
    name:'info',
    components: { 
        Picture 
        },
    data() {
        return {
            esta_trabalhando: false ,
            mostrar_email: true ,
            email:'maylson@moraes',
            meu_link:'https://www.google.com.br/'
        }
    }
    
}
</script>