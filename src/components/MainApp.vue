<template>
    <main class=" text-center">
        <!--WELCOME/ parte 1 -->
        <div class=" py-5 container-c">
            <p class="fw-light fs-1">Welcome to Avada Health</p>
            <p class="container-d fw-light lh-lg">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperium, eaque ipsa quae ab illo</p>
            <div class="row pt-5">
                <cards-app :cards1="cards1"/>
            </div>
        </div>
        <!--WELCOME/ parte 1 -->

        <!--DOCTORS/ parte 2 -->
        <doctor-card />
        <!--DOCTORS/ parte 2 -->

        <!--SERVICES/ parte 3 -->
        <div class="py-5">
            <img src="../assets/images/icon-6.png" alt="">
            <p class="fw-light fs-1">OUR HEALTS SERVICES</p>
            <div class="line-g mx-auto"></div>
            <p class="container-d fw-light lh-lg">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperium, eaque ipsa quae ab illo totam rem aperium, eaque ipsa quae ab illo</p>
            <cards-app-2 :cards2="cards2"/>
                
                
            
        </div>
        <!--SERVICES/ parte 3 -->

        <!--FACILITIES/ parte 4 -->
        
        <div id="jumbotron1">

            <div class="py-5">
            <img src="../assets/images/icon-7.png" alt="">
            <p class="fw-light fs-1">TOUR OUR FACILITIES</p>
            <div class="line-g mx-auto"></div>
            <p class="container-d fw-light lh-lg">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperium, eaque ipsa quae ab illo totam rem aperium, eaque ipsa quae ab illoeaque ipsa quae ab illo totam rem aperium, eaque ipsa quae ab illo</p>
            <img  class="py-3" src="../assets/images/play-icon.png" alt="">
            
        </div>

        </div>
        <!--FACILITIES/ parte 4 -->

        <!--LEARN MORE/ parte 5 -->
        <div class="container-fluid  parte-5">
            <div class="row  ">
                <div class="col-4 box-1 py-5">
                    <h5>Emercency Care</h5>
                    <img class="my-2" src="../assets/images/wave-divider.png" alt="">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit delectus ipsa odit tenetur, soluta quidem?</p>                
                    <a  class="button-w" href=""> LEARN MORE</a>
                </div>
                <div class="col-4 box-2 py-5">
                    <h5>Emercency Care</h5>
                    <img class="my-2" src="../assets/images/wave-divider.png" alt="">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit delectus ipsa odit tenetur, soluta quidem?</p>                
                    <a  class="button-w" href=""> LEARN MORE</a>
                </div>
                <div class="col-4 box-3 py-5">
                    <h5>Emercency Care</h5>
                    <img class="my-2" src="../assets/images/wave-divider.png" alt="">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit delectus ipsa odit tenetur, soluta quidem?</p>                
                    <a  class="button-w" href=""> LEARN MORE</a>
                </div>
                 
            </div>
        </div>
        <!--LEARN MORE/ parte 5 -->

        <!--MAKE/ parte 6 -->
        <div id="jumbotron2">
            <div class="py-5 container-d parte-6">    
                <p class="fw-light fs-1">Make An Appointment</p>
                <div class="line-g mx-auto"></div>
                <p class=" fw-light lh-lg">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperium, eaque ipsa quae ab illo totam rem aperium, eaque ipsa quae ab illoeaque ipsa quae ab illo totam rem aperium, eaque ipsa quae ab illo</p>
                <div class="row text-start">
                    <div class="col-6  my-4">
                        <input type="text" placeholder="name">

                    </div>
                    <div class="col-6 my-4">
                        <input type="email" placeholder="email@">
                    </div>
                    <div class="col-6 my-4">
                        <input type="text" placeholder="telephone number">
                    </div>
                    <div class="col-6 my-4">
                        <input type="date" placeholder="Appointment Date">
                    </div>
                    <div class="col-12 my-4 ">
                        <input type="textarea" placeholder="How can we helmp?" class="text-area">
                    </div>
                    <div class="col-12 my-4">
                        <button>MAKE AN APPOINTMENT</button>
                    </div>
                </div>

            </div>

        </div>
        <!--MAKE/ parte 6 -->

        <!--SPONSOR/ parte 7 -->
        <div class="parte-7">
            <div class="container-c">
                <div class="row">
                    <div class="col-4">
                        <img class="my-2" src="../assets/images/client-logos-1.png" alt="">
                    </div>
                    <div class="col-4">
                        <img class="my-2" src="../assets/images/client-logos-2.png" alt="">
                    </div>
                    <div class="col-4">
                        <img class="my-2" src="../assets/images/client-logos-3.png" alt="">
                    </div>
                    <div class="col-4">
                        <img class="my-2" src="../assets/images/client-logos-4.png" alt="">
                    </div>
                </div>
            </div>
            
            
            
        </div>

        <!--SPONSOR/ parte 7 -->

        
        

        
        

    </main>
</template>

<script>
import CardsApp from './CardsApp.vue';
import DoctorCard from './DoctorCard.vue';
import CardsApp2 from './CardsApp2.vue';

export default {
  
    name:'MainApp',
    components: { 
        DoctorCard,
        CardsApp,
        CardsApp2,

         
    },
     data(){
        return{
            cards1:[
                {
                    title: 'SAME DAY APPOINTMENTS',
                    text: 'Sed ut perspiciatis omnis iste natus error sit voluptam accusantim',
                    image: require('../assets/images/icon-1.png'),
                },
                {
                    title: 'WORLD CLASS FACILITIES',
                    text: 'Sed ut perspiciatis omnis iste natus error sit voluptam accusantim',
                    image: require('../assets/images/icon-2.png'),
                },
                {
                    title: 'EXPERT DOCTORS ',
                    text: 'Sed ut perspiciatis omnis iste natus error sit voluptam accusantim',
                    image: require('../assets/images/icon-3.png'),
                },
                {
                    title: 'COMPLETARY THERAPIES',
                    text: 'Sed ut perspiciatis omnis iste natus error sit voluptam accusantim',
                    image: require('../assets/images/icon-4.png'),
                },
       
            ],
            cards2:[
                {
                    title: 'REHABILITION CENTER',
                    text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.',
                    image: require('../assets/images/icon-14.png'),
                },
                {
                    title: 'DENTAL IMPLANTS',
                    text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.',
                    image: require('../assets/images/icon-15.png'),
                },
                {
                    title: 'MEDICINE RESEARCH',
                    text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.',
                    image: require('../assets/images/icon-16.png'),
                },
                {
                    title: 'BLOOD BANK',
                    text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.',
                    image: require('../assets/images/icon-11.png'),
                },
                {
                    title: 'PHARMACEUTICAL ADVICE',
                    text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.',
                    image: require('../assets/images/icon-12.png'),
                },
                {
                    title: 'MEDICAL COUNSELING',
                    text: 'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.',
                    image: require('../assets/images/icon-13.png'),
                },
                

            ]
            

        }
    },
  
}
</script>

<style lang="scss">
@import '../styles/generals.scss';
.container-social{
    img{
        border-radius: 50%;
    }
    ul{
        padding: 0;
        list-style-type: none;

        li{
            display: inline-block;
            margin-right: 8px;
        }
    }
}
#jumbotron1{
    width: 100%;
    min-height: 546px;
    background-image: url(../assets/images/paralax-bg-tour-facilities.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    color: $text-color-w;
    
}
.parte-5{
    color: $text-color-w;
    width: 100%;
    
    .box-1{
        background-color: #3aafbf;
    }
    .box-2{
        background-color: #3597c3;
    }
    .box-3{
        background-color: #327ec7;
    }
}
#jumbotron2{
    width: 100%;
    min-height: 546px;
    background-image: url(../assets/images/make-an-appointment.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    color: $text-color-w;
    .text-area{
        padding-bottom: 100px;
    }

}
.parte-6{
    input{
        
        width: 100%;
        border: 1px solid white;
        background-color: rgb( 0,0,0,0);
        padding: 10px;
    }
    .box-text{
        height: 100px;
    }
    button{
        width: 100%;
        color: white;
        background-color: #3aafbf;
        padding: 10px;

    }
}
.parte-7{
    width: 100%;
    height: 250px;
    background-image: url(../assets/images/rgb-gradient-bar-for-logo-carrasel.jpg);

}

    



</style>