



<script>
// Js componente
export default {
    name: 'FooterNavComp',
    data() {
        return {
            navSections: [
                {
                    title: 'dc comics',
                    links: [
                        {
                            name: 'Characters',
                            link: '#'
                        },
                        {
                            name: 'Comics',
                            link: '#'
                        },
                        {
                            name: 'Movies',
                            link: '#'
                        },
                        {
                            name: 'TV',
                            link: '#'
                        },
                        {
                            name: 'Games',
                            link: '#'
                        },
                        {
                            name: 'Videos',
                            link: '#'
                        },
                        {
                            name: 'News',
                            link: '#'
                        }
                    ]
                },
                {
                    title: 'shop',
                    links: [
                        {
                            name: 'Shop DC',
                            link: '#'
                        },
                        {
                            name: 'Shop DC Collectibles',
                            link: '#'
                        }
                    ]
                },
                {
                    title: 'dc',
                    links: [
                        {
                            name: 'Terms of Use',
                            link: '#'
                        },
                        {
                            name: 'Privacy policy (New)',
                            link: '#'
                        },
                        {
                            name: 'Ad Choices',
                            link: '#'
                        },
                        {
                            name: 'Advertising',
                            link: '#'
                        },
                        {
                            name: 'Jobs',
                            link: '#'
                        },
                        {
                            name: 'Subscriptions',
                            link: '#'
                        },
                        {
                            name: 'Talent Workshops',
                            link: '#'
                        },
                        {
                            name: 'CPSC Certificates',
                            link: '#'
                        },
                        {
                            name: 'Ratings',
                            link: '#'
                        },
                        {
                            name: 'Shop Help',
                            link: '#'
                        },
                        {
                            name: 'Contact Us',
                            link: '#'
                        }
                    ]
                },
                {
                    title: 'sites',
                    links: [
                        {
                            name: 'DC',
                            link: '#'
                        },
                        {
                            name: 'MAD Magazine',
                            link: '#'
                        },
                        {
                            name: 'DC Kids',
                            link: '#'
                        },
                        {
                            name: 'DC Universe',
                            link: '#'
                        },
                        {
                            name: 'DC Power Visa',
                            link: '#'
                        }
                    ]
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
    <nav>

        <div class="column">
            <div>
                <h3>{{ navSections[0].title }}</h3>
                <ul>
                    <li 
                    v-for="(item, index) in navSections[0].links" :key="index">
                        <a :href="item.link">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <div>
                <h3>{{ navSections[1].title }}</h3>
                <ul>
                    <li 
                    v-for="(item, index) in navSections[1].links" :key="index">
                        <a :href="item.link">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="column">
            <h3>{{ navSections[2].title }}</h3>
            <ul>
                <li 
                v-for="(item, index) in navSections[2].links" :key="index">
                    <a :href="item.link">{{ item.name }}</a>
                </li>
            </ul>
        </div>
        <div class="column">
            <h3>{{ navSections[3].title }}</h3>
            <ul>
                <li 
                v-for="(item, index) in navSections[3].links" :key="index">
                    <a :href="item.link">{{ item.name }}</a>
                </li>
            </ul>
        </div>


        <!-- <div v-for="(element, index) in navSections" :key="index">
            
        </div> -->
    </nav>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../../assets/styles/partials/mixins' as *;
    @use '../../assets/styles/partials/variables' as *;

    nav {
        @include d-flex;
        gap: 20px;

        .column {

            &:first-child {
                display: flex;
                flex-direction: column;
                gap: 20px;

                // border: 1px solid red;
            }

            h3 {
                color: white;
                text-transform: uppercase;
                margin-bottom: 5px;
            }

            ul {
                li {
                    list-style-type: none;

                    a {
                        text-decoration: none;
                        color: $bg-socials_DC;
                        font-size: 0.9rem;

                        &:hover {
                            color: white;
                        }
                    }
                }
            }
        }
    }
    
</style>