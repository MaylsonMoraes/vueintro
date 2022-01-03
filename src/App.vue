<template>
  <header />
  <Primeirocomponente />
  <p class="paragrafo-pai">O dado de app é:{{ testando  }}</p>
  <LifeCycle />
  <Pessoa />
</template>

<script>
import Primeirocomponente from './components/Primeirocomponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import header from './components/header.vue'
export default {
  name: 'App',
  components: {
    Primeirocomponente ,
    LifeCycle ,
    Pessoa,
    header,
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
