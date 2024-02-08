



<script>
// Js componente
export default {
    name: 'SocialsComp',
    data() {
        return {
            socials: [ 'footer-facebook.png', 'footer-periscope.png', 'footer-pinterest.png', 'footer-twitter.png', 'footer-youtube.png' ]
        }
    },
    methods: {
        
    }
}
</script>


<template>
    <!-- html componente -->
    <div>
        <span>follow us</span>
        <ul>
            <li v-for="(social, index) in socials" :key="index">
                <img :src="`../../src/assets/img/${social}`" :alt="social">
            </li>
        </ul>
    </div>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../../assets/styles/partials/mixins' as *;
    @use '../../assets/styles/partials/variables' as *;

    div {
        @include d-flex;
        align-items: center;
        gap: 20px;

        > span {
            text-transform: uppercase;
            font-weight: bold;
            color: $blue_DC;
        }

        ul {
            @include d-flex;
            gap: 10px;

            li {
                list-style-type: none;
            }
        }
    }
    
</style>