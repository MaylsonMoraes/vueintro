<template>
  <Primeirocomponente />
  <p>O dado de app é:{{ testando }}</p>
  <LifeCycle />
  <Pessoa />
</template>

<script>
import Primeirocomponente from './components/Primeirocomponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
export default {
  name: 'App',
  components: {
    Primeirocomponente ,
    LifeCycle ,
    Pessoa
    },
    data(){
      return {
        testando:"teste"
      }
    }
  }
</script>
