<template >
    <div class="bg-teal-200 p-5">
        <p class="bg-[#ffffff] rounded-[20px] pb-4 text-lg md:text-7xl font-bold text-center mt-[20px] "> PokeDEx</p>
        <input class="my-4 rounded-md border-2 border-solid border-[#C2C2C2] focus:border-[#694DF9] outline-none
                active:border-[#E2DCFF] hover:border-[#694DF9] p-1" type="text" placeholder="Buscar Pokemon">
        <div id="container-pokes" class="flex flex-wrap md:gap-[40px] gap-[20px] justify-start">
            
        </div>
    </div>
</template>

<script>
export default {
    name: 'pokeDExPage'
}
</script>

<style></style>