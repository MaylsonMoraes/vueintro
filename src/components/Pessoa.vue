<template>
    
    <h2>Esta é a descrição da Pessoa:{{ nome }}</h2>
    <info />
    <Customform />
    
</template>
<script>
import info from './info'
import Customform from './form'


export default {
    name:'Pessoa',
    components: { 
      info ,
      Customform
    },

    data() {
        return { 
            nome:'Maylson'
        }
    }
}
</script>
