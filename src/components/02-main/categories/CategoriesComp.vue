



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
            <li v-for="(item, index) in categories" :key="index">
                <img :src="`../../../src/assets/img/${item.image}`" alt="">
                <span>{{ item.name }}</span>
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
            width: 100%;

            li {
                @include d-flex;
                width: 100%;
                height: 100%;
                align-items: center;
                
                list-style-type: none;
                color: white;
                text-transform: uppercase;

                img {
                    transform: scale(0.4);
                }

                span {
                    font-size: 0.7rem;
                }
            }
        }
    }

</style>