



<script>
// Js componente
export default {
    name: 'FooterLogoComp',
    data() {
        return {
            
        }
    },
    methods: {
        
    }
}
</script>


<template>
    <!-- html componente -->
    <figure>
        
    </figure>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../../assets/styles/partials/mixins' as *;


    figure {
        height: 100%;
        background-image: url('../../assets/img/dc-logo-bg.png');
        @include bg-image-center-cover;
    }
    
</style>