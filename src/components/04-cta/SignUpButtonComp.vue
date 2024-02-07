




<script>
// Js componente
export default {
    name: 'SignUpButtonComp',
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
    <button>sign-up now!</button>
    
</template>


<style lang="scss" scoped>
    /* stile del componente */

    @use '../../assets/styles/partials/mixins' as *;
    @use '../../assets/styles/partials/variables' as *;

    button {
        @include btn;
        @include btn-transparent-blue;        
    }
    
</style>