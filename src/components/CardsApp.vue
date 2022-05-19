<template>
        <div class="row pt-5">
         
            <div class="col-3 col-lg-3 col-md-6 col-sm-12" v-for="(card,i) in cards1" :key="i">       
                <img :src="card.image"  alt="">
                <p class="fw-light fs-6">{{card.title}}</p>
                <p class="fw-light fs-6">{{card.text}}</p>
                    
            </div>
                
        </div>
    
</template>

<script>
export default {
    name:'CardsApp',
    props:["cards1"],
    data(){
        return{

        }
    },
}
</script>

<style lang="scss">

</style>