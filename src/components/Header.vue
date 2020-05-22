<template>
    <div>        
        <Topnav />                  
    </div>
</template>

<script>
import Topnav from '../components/subcomponents/Topnav.vue';
import CollapsibleMenu from '../components/subcomponents/CollapsibleMenu.vue';

    export default {
        name: 'Header',
        components: {
            Topnav, CollapsibleMenu
        }
    };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



</style>

