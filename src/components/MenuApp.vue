<template>
    <div class="menu d-lg-none">
    <menu-item 
    v-for="(item,index) in menuTree"
    :key="index"
    :label="item.label"
    :depth="0"
    :data="item.children"

    />
    </div>
</template>

<script>
import MenuItem from './MenuItem.vue';
export default {
    name:"recursive-menu",
    components:{
        MenuItem,
    },
    data(){
        return{
            menuTree:[
                {
                    label:"MENU",
                    icon:"home",
                    children:[
                        {
                            label: "HOME",
                        },
                        {
                            label: "ABOUT",
                        },
                        {
                            label: "DEPARTMENTS",
                        },
                        
                    ]
                },
                
            ]

        }
    }
    
}
</script>

<style lang="scss">
.menu{
    padding-top: 20px;

    
    width: 240px;
    
    
    transition:  all .3s ease;
    overflow: auto;
    
}

</style>