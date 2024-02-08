


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
        change(index) {
            this.navLinks.forEach(element => {
                if (element.selected) {
                    element.selected = false;
                }
                this.navLinks[index].selected = true;
            });
        }
    }
}
</script>


<template>
    <!-- html componente -->
    <nav>
        <ul>
            <li 
            v-for="(element, index) in navLinks"
            :class="element.selected ? 'active' : ''"
            @click="change(index)">
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
        height: 100%;

        ul {
            @include d-flex;
            // align-items: center;
            gap: 1rem;
            height: 100%;
            
            li {
                @include d-flex;
                align-items: center;

                list-style-type: none;
                text-transform: uppercase;
                height: 100%;
                border-bottom: 3px solid transparent;

                a {
                    text-decoration: none;
                    color: $black_DC;

                    &:hover {
                        color: $blue_DC;
                    }
                }
            }
        }
    }

    .active {
        border-bottom: 3px solid $blue_DC;

        a {
            color: $blue_DC;
        }
    }
    
</style>