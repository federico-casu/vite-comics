<!-- 

  Descrizione:
  Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
  Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
  Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!

  Bonus:
  Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.

-->

<script>
  import HeaderComp from './components/HeaderComp.vue';
  import ContentComp from './components/02-main/ContentComp.vue';


  export default {
    components: {
      HeaderComp,
      ContentComp
    }
  }
</script>

<template>
  
  <header>
    <HeaderComp/>
  </header>

  <main>
    <ContentComp/>
  </main>

  <footer>

  </footer>

</template>

<style lang="scss">

@use './assets/styles/general.scss' as *;
@use './assets/styles/partials/mixins' as *;
@use './assets/styles/partials/variables' as *;

header {
  border: 1px solid red;
}

main {
  background-color: $black_DC;

  height: 15vh;
}

</style>
