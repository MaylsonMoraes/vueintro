<template>
  <Primeirocomponente/>
  <LifeCycle/>
</template>

<script>
import Primeirocomponente from './components/Primeirocomponente.vue'
import LifeCycle from './components/LifeCycle.vue'
export default {
  name: 'App',
  components: {
    Primeirocomponente ,
    LifeCycle
  }
  }
</script>
