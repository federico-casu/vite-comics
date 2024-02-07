



<script>
// Js componente

import SignUpButtonComp from './SignUpButtonComp.vue';
import SocialsComp from './SocialsComp.vue';

export default {
    name: 'CTAComp',
    data() {
        return {

        }
    },
    methods: {

    },
    components: {
        SignUpButtonComp,
        SocialsComp
    }
}
</script>


<template>
    <!-- html componente -->

    <div class="container">
        <SignUpButtonComp/>
        <SocialsComp/>
    </div>
</template>


<style lang="scss" scoped>
/* stile del componente */

@use '../../assets/styles/partials/mixins' as *;

.container {
    height: 100%;
    @include d-flex;
    justify-content: space-between;
    align-items: center;
}
</style>