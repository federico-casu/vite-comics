



<script>
// Js componente

import FooterNavComp from './03-footer/FooterNavComp.vue';
import FooterLogoComp from './03-footer/FooterLogoComp.vue';

export default {
    name: 'FooterComp',
    data() {
        return {
            
        };
    },
    methods: {},
    components: {
        FooterNavComp,
        FooterLogoComp
    }
}
</script>


<template>
    <!-- html componente -->
    <div class="container">
        <FooterNavComp/>
        <div>
            <FooterLogoComp/>
        </div>
    </div>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../assets/styles/partials/mixins' as *;

    .container {
        border: 1px solid lime;
        height: 100%;

        @include d-flex;
        justify-content: space-between;
        align-items: center;

        > div {
            height: 100%;
            width: 45%;
        }
    }
    
</style>