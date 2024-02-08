



<script>
// Js componente
export default {
    name: 'ComicComp',
    data() {
        return {
            
        }
    },
    methods: {
        
    },
    props: {
        thumb: String,
        series: String
    }
}
</script>


<template>
    <!-- html componente -->
    <div>
        <figure>
            <img :src="thumb" :alt="series">
        </figure>
        <span>{{ series }}</span>
    </div>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../../assets/styles/partials/mixins' as *;
    @use '../../assets/styles/partials/variables' as *;

    div {
        flex-basis: calc(100% / 6 - (100px / 6 ));
        height: 300px;
        @include d-flex;
        flex-direction: column;
        gap: 10px;
        cursor: pointer;

        &:hover {
            > span {
                color: $blue_DC;
            }
        }

        figure {
            img {
                height: 200px;
                width: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
    }
    
</style>