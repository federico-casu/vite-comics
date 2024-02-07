



<script>
// Js componente
export default {
    name: 'SocialsComp',
    data() {
        return {
            socials: [ '../../assets/img/footer-facebook.png', '../../assets/img/footer-periscope.png', '../../assets/img/footer-pinterest.png', '../../assets/img/footer-twitter.png', '../../assets/img/footer-youtube.png' ]
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
            <li><img src="../../assets/img/footer-facebook.png" alt=""></li>
            <li><img src="../../assets/img/footer-periscope.png" alt=""></li>
            <li><img src="../../assets/img/footer-pinterest.png" alt=""></li>
            <li><img src="../../assets/img/footer-twitter.png" alt=""></li>
            <li><img src="../../assets/img/footer-youtube.png" alt=""></li>
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