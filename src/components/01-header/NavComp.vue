


<script>
// Js componente
export default {
    name: 'NavComp',
    data() {
        return {
            navLinks: [
                {
                    name: 'characters',
                    link: '#',
                    selected: false
                },
                {
                    name: 'comics',
                    link: '#',
                    selected: false
                },
                {
                    name: 'movies',
                    link: '#',
                    selected: false
                },
                {
                    name: 'tv',
                    link: '#',
                    selected: false
                },
                {
                    name: 'games',
                    link: '#',
                    selected: false
                },
                {
                    name: 'collectibles',
                    link: '#',
                    selected: false
                },
                {
                    name: 'videos',
                    link: '#',
                    selected: false
                },
                {
                    name: 'fans',
                    link: '#',
                    selected: false
                },
                {
                    name: 'news',
                    link: '#',
                    selected: false
                },
                {
                    name: 'shop',
                    link: '#',
                    selected: false
                },
            ]
        }
    },
    methods: {
        
    }
}
</script>


<template>
    <!-- html componente -->
    <nav>
        <ul>
            <li 
            v-for="(element, index) in navLinks">
                <a :href="element.link">{{ element.name }}</a>
            </li>
        </ul>
    </nav>
    
</template>



<style lang="scss" scoped>
    @use '../../assets/styles/partials/mixins' as *;
    @use '../../assets/styles/partials/variables' as *;

    /* stile del componente */
    nav {
        ul {
            @include d-flex;
            gap: 1rem;
            li {
                list-style-type: none;
                text-transform: uppercase;
                
                a {
                    text-decoration: none;
                    color: $black_DC;
                }
            }
        }
    }
    
</style>