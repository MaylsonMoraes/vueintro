<template>
    
    <h2>Esta é a descrição da Pessoa:{{ nome }}</h2>
    <info />
    <form />
    
</template>
<script>
import info from './info'
import form from './form'

export default {
    name:'Pessoa',
    components: { 
      info ,
      form
  },

data() {
return { 
    nome:'Maylson'
    }
}
}
</script>
