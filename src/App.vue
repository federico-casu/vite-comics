<!-- 

  Descrizione:
  Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
  Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
  Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!

  Bonus:
  Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.

-->

<script>
  import LogoComp from './components/01-header/LogoComp.vue';

  export default {
    components: {
      LogoComp
    }
  }
</script>

<template>
  
  <header>
    <div class="container">
      <LogoComp/>
    </div>
  </header>

  <main>

  </main>

  <footer>

  </footer>

</template>

<style lang="scss">

@use './assets/styles/general.scss' as *;
@use './assets/styles/partials/mixins' as *;

header {
  .container {
    @include d-flex;
    justify-content: space-between;
    align-items: center;

    padding: 1rem 0;
  }

  border: 1px solid red;
}

</style>
