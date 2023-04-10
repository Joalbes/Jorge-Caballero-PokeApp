<template >
    <div class="bg-teal-200 p-5">
        <p class="bg-[#ffffff] rounded-[20px] pb-4 text-lg md:text-7xl font-bold text-center mt-[20px] "> PokeDEx</p>
        <input class="my-4 rounded-md border-2 border-solid border-[#C2C2C2] focus:border-[#694DF9] outline-none
            active:border-[#E2DCFF] hover:border-[#694DF9] p-1" type="text" placeholder="Buscar Pokemon">
        <div id="container-pokes" class="flex flex-wrap md:gap-[40px] gap-[20px] justify-start">
            <div id="card-bulbasaur"
                class="card bg-red-600 rounded-md border-4 border-solid border-[#ffffff] shadow-lg shadow-black hover:cursor-pointer">
                <div class="p-4">
                    <img class="w-[250px] h-[250px] rounded-md" src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/official-artwork/shiny/1.png" alt="sus">
                </div>
                <div>
                    <p class="font-bold italic text-center text-2xl text-[#ffffff] p-2">bulbasaur</p>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'pokeDExPage'
}
</script>

<style></style>