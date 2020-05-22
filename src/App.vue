<template>
    <div id="app">            
        <Header />         
        <Emulation />
    </div>
</template>

<script>
    import Home from './components/Home.vue';    
    import Emulation from './views/Emulation.vue';
    import Models from './views/Models.vue';
    import Header from './components/Header.vue';
    import Plotly from 'vue-plotly';

    export default {
        name: 'app',
        components: {
            Home, 
            Emulation,
            Models,
            Header,
            Plotly     
        }
    };
</script>

<style>
</style>

