<template>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{nome}} e trabalho como {{profissao}}.</p>
    <multiplosEventos />
</template>

<script>
import multiplosEventos from './multiplosEventos.vue';
export default {
    name: 'Primeirocomponente',
    components: {
        multiplosEventos
    },
    data() {
        return{
            nome:"Maylson",
            profissao: "Programador"
        }
    }
}
</script>
