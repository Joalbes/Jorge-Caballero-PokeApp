<template>
    <NuxtLink :to="{path:nombre, query:{imagen:url} }" class="w-[18%] h-[1/2] bg-gray-200 flex flex-col justify-center items-center">
        <img :src="url" >
        <p>{{ nombre }}</p>
    </NuxtLink>
</template>
<script>
import path from 'path';

export default{
    props:{
        nombre:{
            type:String,
            required:true
        },
        url:{
            type:String,
            required: true
        }
    }
}</script>
<style></style>