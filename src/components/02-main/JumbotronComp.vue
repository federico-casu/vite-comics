



<script>
// Js componente
export default {
    name: 'JumbotronComp',
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
        <img src="../../assets/img/jumbotron.jpg" alt="">
    </figure>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    figure {
        max-height: 40vh;

        img {
            max-height: 40vh;
            width: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
    
</style>