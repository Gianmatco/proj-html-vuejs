<template>
    <div class="menu-item">
        
        <div class="label" @click="togglerMenu">
            <i v-if="icon" class="material-icons">{{icon}}</i>
            <span>{{label}}</span>
        </div>
        <div v-show="showChildren" class="items-container">
            <menu-item v-for="(item,index) in data"
            :key="index"
            :label="item.label"
            :depth="depth + 1"
            :data="item.children"
             />
        </div>
    </div>
</template> 

<script>
export default {
    name:"menu-item",
    data(){
        return{
            showChildren: false,

        }

    },
    props:{
        label:{
            type: String,
            required: true,
        },
        icon:{
            type: String,
        },
        depth:{
            type: Number,
            required:true,
        },
        data:{
            type: Array
        }
    },
    methods:{
        togglerMenu(){
            this.showChildren = !this.showChildren

        }
    }
}
</script>