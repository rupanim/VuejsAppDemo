<template>
    <div id="" class="row col-sm-12" style="padding-right: 0px; padding-top: 0px;width:">
        <div class="collapse navbar-collapse col-sm-1 navbar-dark bg-dark" id="navbarToggleExternalContent">
                    <ul class="navbar-nav">
                        <li class="nav-item active">
                            <a class="nav-link" href="#">Emulation </a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Models</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">Help</a>
                        </li>
                    </ul>    
            </div> 
    </div>    
</template>

<script>
    export default {
        name: 'Topnav'
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

