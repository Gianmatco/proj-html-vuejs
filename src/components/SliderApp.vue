<template>
<div class="wrapper">
    <div class="slider-app" :style="{'margin-left': '-' +(100*currentSliderIndex)+ '%'}">
        <slider-item v-for="item in slider_data" :key="item.id" :item_data="item"/>
    </div>
    

</div>
    
</template>

<script>
import SliderItem from './SliderItem.vue';



export default {
    
    name:"SliderApp",
    props:{
        slider_data:{
            type: Array,
            default: ()=>[]
        },
        interval:{
            type: Number,
            default: 0
        },

    },
    components:{
        SliderItem
       
        
    },
    methods:{
        prevSlider(){
            if(this.currentSliderIndex > 0){
                this.currentSliderIndex--
            }
        },
        nextSlider(){
            if(this.currentSliderIndex >= this.slider_data.length - 1){
                this.currentSliderIndex = 0

            }else{
                this.currentSliderIndex++
            }
            
        } 

        

    },
    mounted(){
        if(this.interval > 0){
            let vm = this
            setInterval(function(){
            vm.nextSlider()    
            },vm.interval)
        }

    },
    data(){
        return{
            currentSliderIndex:0,
        }
    }
    
    
}
</script>

<style lang="scss">
.wrapper{
    
    overflow: hidden;
    max-width: 300px;
    margin: 0 auto;
}
.slider-app{
    display: flex;
    transition: all ease .3s;
}

</style>