



<script>
// Js componente
export default {
    name: 'ContentComp',
    data() {
        return {
            message: "-->Content goes here<--"
        }
    },
    methods: {
        
    }
}
</script>


<template>
    <!-- html componente -->
    <div class="container">
        <h1>{{ message }}</h1>
    </div>
    
    
</template>


<style lang="scss" scoped>
    /* stile del componente */
    @use '../../assets/styles/partials/variables' as *;
    @use '../../assets/styles/partials/mixins' as *;

    .container {
        color: white;
        height: 100%;

        @include d-flex;
        align-items: center;
    }

    
</style>