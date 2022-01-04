<template>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{nome}} e trabalho como {{profissao}}.</p>
    <multiplosEventos />
    <reutilizacao />
</template>

<script>
import multiplosEventos from './multiplosEventos.vue';
import reutilizacao from './reutilizacao.vue';
export default {
    name: 'Primeirocomponente',
    components: {
        multiplosEventos,
        reutilizacao,
        
    },
    data() {
        return{
            nome:"Maylson",
            profissao: "Programador"
        }
    }
}
</script>
