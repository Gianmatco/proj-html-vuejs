<template>
<div id="jumbotron">
    <nav class="container-fluid"><!-- navbar-->
        <div class="row p-4 ">
            <div class="col-5">
            <img src="../assets/images/medical_logo_1x_light.png" alt="" width="50%">
            </div>
            <div class="col-7">
                <ul class="d-flex justify-content-end">
                    <li><a href="">home</a></li>
                    <li><a href="">departments</a></li>
                    <li><a href="">articles</a></li>
                    <li><a href="">carticles</a> </li>
                    <li><a href="" class="button-b">make appointment</a></li>
                </ul>
            </div>  
            
        </div>
        
    </nav>
    <!-- navbar-->


    <!-- navbar-->
    <nav class="navbar navbar-expand-lg ">
    <div class="container-fluid d-flex justify-content-center">
        <div class="row">
            <div class="col-4">
                <a class="navbar-brand" href="#">
                    <img src="../assets/images/medical_logo_1x_light.png" alt=""  class="d-inline-block align-text-top">
                </a>
            </div>
            <div class="col-8">
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto mb-2 mb-lg-0 d-flex justify-content-end">
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">departments</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">articles</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">carticles</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link button-b" href="#">make appointment</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                Dropdown
                            </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                            <li><a class="dropdown-item" href="#">Action</a></li>
                            <li><a class="dropdown-item" href="#">Another action</a></li>
                            <li><hr class="dropdown-divider"></li>
                            <li><a class="dropdown-item " href="#">Something else here</a></li>
                        </ul>
                        </li>
                        
                    </ul>
                </div>

            </div>
        </div>
        
        
        
    </div>
    </nav>
    <!-- navbar-->
    <div class="container-c mt-5 pt-5">

        
            <div class="card-body ">
                <h1 class="card-title">Caring For Life</h1>
                <p class="card-text my-4">Kids words con be short and easy to speak, but their echoes are truly endless. Avada health focuses on you as if it was our own family.</p>
                <a href="#" class="button-b">learn more</a>
            </div>
        

       
    </div>
</div>


</template>

<script>
export default {
    name:'NavBar',
    
}
</script>

<style lang="scss">
@import '../styles/generals.scss';

#jumbotron{
    width: 100%;
    min-height: 546px;
    background-image: url(../assets/images/header-image-homepage.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    color: $text-color-w;
    

}
nav{
   
    ul{

        list-style-type: none;
        li{
            display: inline-block;
            margin: 0 15px;
            text-decoration: none;

            a{
                color: $text-color-w;  
                text-decoration: none;
            }
        }
    }
}
.card-body{
    width: 600px;

}




</style>