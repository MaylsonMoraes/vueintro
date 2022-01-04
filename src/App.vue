<template>
  <Header :esta_logado="true"/>
  <Primeirocomponente />
  <p class="paragrafo-pai">O dado de app é:{{ testando  }}</p>
  <LifeCycle />
  <Pessoa />
</template>

<script>
import Header from './components/Header.vue'
import Primeirocomponente from './components/Primeirocomponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
export default {
  name: 'App',
  components: {
    Primeirocomponente ,
    LifeCycle ,
    Pessoa,
    Header
    },
    data(){
      return {
        testando:"teste"
      }
    }
  }
</script>

<style>
  body {
    background-color: #333;
    color: #fff;
  }

  a {
    color: red;
  }
  .teste {
    background-color: #000;
  }
</style>
