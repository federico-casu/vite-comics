



<script>
// Js componente
export default {
    name: 'CategoriesComp',
    data() {
        return {
            categories: [
                {
                    name: 'digital comics',
                    image: 'buy-comics-digital-comics.png'
                },
                {
                    name: 'dc merchandise',
                    image: 'buy-comics-merchandise.png'
                },
                {
                    name: 'subscription',
                    image: 'buy-comics-subscriptions.png'
                },
                {
                    name: 'comic shop locator',
                    image: 'buy-comics-shop-locator.png'
                },
                {
                    name: 'dc power visa',
                    image: 'buy-dc-power-visa.svg'
                }
            ]
        }
    },
    methods: {
        
    }
}
</script>


<template>
    <!-- html componente -->
    <div class="container">
        <ul>
            <li>
                <img src="../../../assets/img/buy-comics-digital-comics.png" alt="">
                <span>digital comics</span>
            </li>
            <li>
                <img src="../../../assets/img/buy-comics-merchandise.png" alt="">
                <span>dc merchandise</span>
            </li>
            <li>
                <img src="../../../assets/img/buy-comics-subscriptions.png" alt="">
                <span>subscription</span>
            </li>
            <li>
                <img src="../../../assets/img/buy-comics-shop-locator.png" alt="">
                <span>comic shop locator</span>
            </li>
            <li>
                <img src="../../../assets/img/buy-dc-power-visa.svg" alt="">
                <span>dc power visa</span>
            </li>
        </ul>
    </div>

    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../../../assets/styles/partials/mixins' as *;

    .container {
        @include d-flex;
        height: 100%;
        align-items: center;

        ul {
            @include d-flex;
            align-items: center;

            li {
                @include d-flex;
                align-items: center;
                list-style-type: none;

                img {
                    transform: scale(0.4);
                }
            }
        }
    }

</style>