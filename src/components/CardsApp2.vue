<template>
<div class="row pt-5 mx-auto  d-flex justify-content-around p-2">
    <div class=" col-4 col-lg-4 col-md-5 col-sm-12 bg-white p-3  " v-for="(card,i) in cards2" :key="i">
        <img :src="card.image">
        <div class="lh-s">
            <div class="mt-3">
                <h3 class="fw-light fs-6">{{card.title}}</h3>                                
                <p>{{card.text}}</p>
            </div>
    
        </div>          
    </div>
</div>   
</template>

<script>
export default {
    name:'CardsApp2',
    props:["cards2"],
    data(){
        return{

        }
    },
}
</script>

<style lang="scss">

</style>