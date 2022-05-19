<template>
<div id="jumbotron">
    



    
    <!-- navbar-->
    <nav class="navbar navbar-expand-lg pt-4">
            <div class="container-fluid d-flex justify-content-between">
                <a class="navbar-brand gap-5" href="#">
                   <img src="../assets/images/medical_logo_2x_light.png" alt="" width="200">
                </a>
                
                
                <div class="d-flex align-items-end flex-column " >
                    
                    
                    <menu-app/>
                   
                    <div class="p-2">
                            <div class="collapse navbar-collapse " id="navbarSupportedContent">
                                <ul class="navbar-nav me-auto mb-2 mb-lg-0  ">
                                    <li class="nav-item">
                                        <a class="nav-link active" aria-current="page" href="#">HOME</a>
                                    </li>
                                    <li class="nav-item pt-2">
                                        <a class="" href="#">ABOUT</a>
                                    </li>
                                    
                                    <li class="nav-item pt-2">
                                        <a class="" href="#">DEPARTMENTS</a>
                                    </li>
                                    <li class="nav-item pt-2">
                                        <a class="" href="#">ARTICLES</a>
                                    </li>
                                    <li class="nav-item pt-2">
                                        <a class="" href="#">DEPARTMENTS</a>
                                    </li>
                                    <li class="nav-item pt-2">
                                        <a class=" button-b" href="#">MAKE APPOINTMENT</a>
                                    </li>
                        
                                </ul>
                
                            </div>
                    </div>     
                </div>
            </div>
    </nav>
    <!-- navbar-->

    
    <div class="container-c my-5 pt-5">
        <div class="row ">
            <div class="card-body mb-5 pb-5">
                <h1 class="card-title">Caring For Life</h1>
                <p class="card-text my-4">Kids words con be short and easy to speak, but their echoes are truly endless. Avada health focuses on you as if it was our own family.</p>
                <a href="#" class="button-b">learn more</a>
            </div>
        </div>

        
            
        

       
    </div>
</div>


</template>

<script>
import MenuApp from './MenuApp.vue';

export default {
    name:'NavBar',
    components:{
       MenuApp,
        
    },
    data(){
        return{
            

        }
    },
    methods:{
        handleView(){
            this.mobileView = window.innerWidth <= 990;
        }

    },
    created(){
        this.handleView();
    }
    
}
</script>

<style lang="scss">
@import '../styles/generals.scss';

#jumbotron{
    width: 100%;
    
    background-image: url(../assets/images/header-image-homepage.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    color: $text-color-w;
    

}
nav{
    .h-menu{
        
        color: $text-color-w;
        border: 1px solid $text-color-w;
        
    }
   
    ul{
        margin-right:10px;
        list-style-type: none;
        
        li{
            display: inline-block;
            margin: 0 15px;
            font-size: 12px;
            text-decoration: none;

            a{
                color: $text-color-w;  
                text-decoration: none;
                
                
            }
        }
    }
    .open{
        transform: translatex(8px);
    }
}
.card-body{
    width: 600px;

}




</style>