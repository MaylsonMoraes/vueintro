<template>
    <img :src="avatar" :alt="descricao">
    <reutilizacao />
</template>
<script>
import reutilizacao from '../reutilizacao.vue'

export default {
    name:'Picture',
    components: {
        reutilizacao
    },
    data() {
  
          return {
            avatar:"/img/download.jpeg",
            descricao: "Teste"
        }
    }
}
</script>