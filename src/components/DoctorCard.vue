<template>
    <div class="py-5  container-color-g">
        <img src="../assets/images/icon-5.png" alt="">
        <p class="fw-light fs-1">MEET OUR DOCTORS</p>
        <div class="line-g mx-auto"></div>
        <p class="container-d fw-light lh-lg">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperium, eaque ipsa quae ab illo</p>
        <div class="row pt-5 mx-auto container-c d-flex justify-content-around gap-1">
            <div  class=" col-3  bg-white p-0 " v-for="card in cards" :key="card">
                <img :src="card.image"  width="100%">
                <div class="lh-s text-start p-3">
                    <div>
                        <h3 class="fw-light fs-6">{{card.name}}</h3>
                        <p class="fw-light fs-6">{{card.job}}</p>
                    </div>
                    <div class="fw-light fs-6 ">
                        <p>{{card.text}}</p>
                    </div>
                    <div class="container-social">
                        <ul>
                            <li>
                                <a href=""><img src="../assets/images/twitter.jpg"  width="30px" alt=""></a>
                            </li>
                            <li>
                                <a href=""><img src="../assets/images/youtube.png"  width="30px" alt=""></a>
                            </li>
                            <li>
                                <a href=""><img src="../assets/images/instagram.jpg"  width="30px" alt=""></a>
                            </li>
                        </ul>
                    </div>
                                
                </div>          
            </div>
        </div>    
    </div>
</template>

<script>
export default {
    name:'DoctorCard',
    data(){
        return{
            cards:[
                {
                    name: 'JON SNOW',
                    job: 'Anesthesiologist',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, maiores!',
                    image: require('../assets/images/doctor-1.jpg')
                },
                {
                    name: 'TONY STARK',
                    job: 'Cardiologist',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, maiores!',
                    image: require('../assets/images/doctor-2.jpg')
                },
                {
                    name: 'CAPITAN AMERICA',
                    job: 'Nurse Practitioner',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, maiores!',
                    image: require('../assets/images/doctor-3.jpg')
                }
            ]
            

        }
    },
    methods:{
        
    }
    
}
</script>

<style lang="scss">

</style>