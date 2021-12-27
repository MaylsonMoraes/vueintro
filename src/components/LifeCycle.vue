<template>
    <h1>Meu nome é:{{nome}} </h1>
</template>

<script>
export default {
    name: 'LifeCycle.vue',
    data() {
        return{
            nome:'Ainda não'
        }
    },
    created(){
        setTimeout(()=>{
            this.nome = 'Maylson'
        },1000);
    },
    mounted(){
        setTimeout(()=>{
            this.nome = 'Moraes'
        },2000) 
        
    }
}
</script>
