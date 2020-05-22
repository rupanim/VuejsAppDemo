<template>
    <div>
       <!-- <plotly :data='data' :layout='layout' /> -->
    </div>    
</template>

<script>

    export default {
        name: 'Topnav',
        components: {
            
        },
        data() {
            return {
                data :[{
                    x: [1,2,3,4],
                    y: [10,15,13,17],
                    type:"scatter"
                }],
                layout:{
                title: "My graph"
                }
            }
  }
    };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

#layer2{
position: absolute; 
z-index: 2
}

.border {
    background-color: black;
}
.navbar .anritsuLogo {
    background: url(../../../public/images/anritsulogo.png) no-repeat left center !important;
}

.glyphicon-menu-hamburger {
  font-size: npx;
}
</style>

