<template>
<div>
    <div class="navbar navbar-dark bg-dark row col-sm-12" style="padding-right: 0px; padding-top: 0px">
        <div class="col-sm-1">
            <nav class="">            
                 <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarToggleExternalContent" aria-controls="navbarToggleExternalContent" aria-expanded="true" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>                           
            </nav>            
        </div>
        <div class="col-sm-11">
            <nav class="navbar-dark bg-dark">   
                <a href="https://www.anritsu.com" target="_blank">
                    <img src="../../../public/images/anritsulogo.png"  href="https://www.anritsu.com" target="_blank"   />  
                </a>        
            </nav>            
        </div>       
    </div>
    
    <div>
        <div id="layer2" class="row col-sm-12" style="padding-right: 0px; padding-top: 0px;">
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

#outerLayer{
position: relative; 
z-index: 0
}

#layer1{
position: absolute; 
z-index: 1
}

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

