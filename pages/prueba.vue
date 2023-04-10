<template> 
<div>
    <p class="text-4xl"> {{ name }}</p>
    <!-- <figure v-if="name" >
        <img src="ferrari-sp48-unica.webp" alt="" srcset="">
    </figure> -->

    <button @click="cambiar">Cambiar Nombre</button>
</div>
</template>

<script>
export default {
    name:"pruebaPage",
    data(){
        return{
            name:'Jorge',
            mostrar:true
        }
    },
    methods:{
        cambiar(){
            this.name = 'Caballero'
        }
    }
} </script>


<style> 
    button{
        background-color:red;
    }
</style>