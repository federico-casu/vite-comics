



<script>
// Js componente

import LogoComp from './01-header/LogoComp.vue';
import NavComp from './01-header/NavComp.vue';

export default {
    name: 'HeaderComp',
    components: { 
        LogoComp,
        NavComp 
    },
    data() {
        return {

        };
    },
    methods: {

    }
}
</script>


<template>
    <!-- html componente -->
    <div class="container">
      <LogoComp/>
      <NavComp/>
    </div>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../assets/styles/partials/mixins' as *;

    .container {
        @include d-flex;
        justify-content: space-between;
        align-items: center;

        padding: 1rem 0;

        // border: 1px dashed black;
    }
    
</style>