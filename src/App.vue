<!-- 

  Descrizione:
  Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
  Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
  Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!

  Bonus:
  Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.

  ------------------------------------------------------------------------------------------------------------------------------

  Descrizione:
  Continuate a lavorare nella stessa repo di ieri e create un nuovo componente che rappresenterà le card dei fumetti.
  Utilizzate i dati presenti nel file json che trovate in allegato e passateli al componente Card tramite props.

  Una volta inseriti tutti i contenuti dinamicamente, completate il vostro layout e rifinite i dettagli con Sass.

  Attenzione: Usare i dati degli oggetti presenti nello zip chiamato: "dc-comics.zip" e non quelli presenti nell'altra cartela chiamata "vue-dc-comics-2.zip"

-->

<script>
  import HeaderComp from './components/HeaderComp.vue';
  import ContentComp from './components/02-main/ContentComp.vue';
  import FooterComp from './components/FooterComp.vue';
  import CTAComp from './components/04-cta/CTAComp.vue';
  import CategoriesComp from './components/02-main/categories/CategoriesComp.vue';


  export default {
    components: {
      HeaderComp,
      ContentComp,
      FooterComp,
      CTAComp,
      CategoriesComp
    }
  }
</script>

<template>
  
  <header>
    <HeaderComp/>
  </header>

  <main>
    <section class="content">
      <ContentComp/>
    </section>

    <section class="categories">
      <CategoriesComp/>
    </section>
  </main>

  <footer>
    <FooterComp/>
  </footer>

  <div id="cta">
    <CTAComp/>
  </div>

</template>

<style lang="scss">

@use './assets/styles/general.scss' as *;
@use './assets/styles/partials/mixins' as *;
@use './assets/styles/partials/variables' as *;


main {
  .content {
    background-color: $black_DC;
    // height: 15vh;
  }

  .categories {
    background-color: $blue_DC;
    // height: 15vh;
  }
}

footer {
  background-image: url('./assets/img/footer-bg.jpg');
  @include bg-image-top-cover;
  height: 280px;
}

#cta {
  background-color: $dark-grey_DC;
  height: 15vh;
}

</style>
