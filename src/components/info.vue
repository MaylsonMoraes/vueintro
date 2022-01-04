<template>
<div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades!</p>
    <p>Utilizo as seguintes tecnologias para back-end:</p>
    <ul>
        <li v-for="(technology, index) in backend_technologies" v-bind:key="index">
            {{ technology }}
            </li>
    </ul>
    <p>Utilizo as seguintes tecnologias para front-end:</p>
    <ul>
        <li v-for="technology in frontend_technologies" :key="technology.id">
            {{ technology.language }}
        </li>
    </ul>
    <div>
        <button @click="showMail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para:{{ email }}</p>
    <p class="teste">Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">Basta clicar aqui</a></p>
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
        props: {
            email: String,
            esta_trabalhando: Boolean
        },
    data() {
        return {
            mostrar_email: false ,
            meu_link:'https://www.google.com.br/',
            textoBotao: 'Mostrar E-mail',
            backend_technologies: ['JavaScript','PHP','Python'],
            frontend_technologies: [
                {id:1, language:'HTML'},
                {id:2, language:'CSS'},
                {id:3, language:'Vue'}
            ]
        }
        
    } ,
    methods: {
        showMail() {
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email) {
                this.textoBotao = 'Mostrar E-mail'
            } else {
                this.textoBotao = 'Ocultar E-mail'
            }
        }
    }    
}
</script>

<style>
.paragrafo-pai {
    color:red;
}
</style>