<template>
<div id="jumbotron">
    <nav class="container-fluid"><!-- navbar-->
        <div class="row p-3 ">
            <div class="col-5">
            <img src="../assets/images/medical_logo_1x_light.png" alt="" width="50%">
            </div>
            <div class="col-7">
                <ul class="d-flex justify-content-end">
                    <li><a href="">home</a></li>
                    <li><a href="">departments</a></li>
                    <li><a href="">articles</a></li>
                    <li><a href="">carticles</a> </li>
                    <li><a href="">make appointment</a></li>
                </ul>
            </div>  
            
        </div>
        
    </nav><!-- navbar-->
    
        <div class="card ">
            <div class="card-body">
                <h5 class="card-title">Caring For Life</h5>
                <p class="card-text">Kids words con be short and easy to speak, but their echoes are truly endless. Avada health focuses on you as if it was our own family.</p>
                <a href="#" class="btn btn-primary">learn more</a>
            </div>
        </div>
    
    
   


</div>


</template>

<script>
export default {
    
}
</script>

<style lang="scss">
#jumbotron{
    width: 100vw;
    min-height: 546px;
    background-image: url(../assets/images/header-image-homepage.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;

}
nav{
   
    ul{

        list-style-type: none;
        li{
            display: inline-block;
            margin: 0 15px;
            text-decoration: none;

            a{
                color: white;  
                text-decoration: none;
            }
        }
    }
}
.card{
    width: 80vh;
}

</style>