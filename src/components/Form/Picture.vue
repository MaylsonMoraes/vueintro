<template>
    <img :src="avatar" :alt="descricao">
    <MudarImagem @mudar-imagem="trocarImagem"/>
    
</template>
<script>
import reutilizacao from '../reutilizacao.vue'
import MudarImagem from '../MudarImagem.vue'

export default {
    name:'Picture',
    components: {
        reutilizacao,
        MudarImagem
    },
    data() {
  
          return {
            avatar:"/img/download.jpeg",
            descricao: "Teste"
        }
    },
    methods: {
        trocarImagem() {
            this.avatar = "/img/avatar.png"
        }
    }
}
</script>