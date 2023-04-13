<template>
    <div class="flex flex-row bg-red-200 h-screen p-[2rem]">
        <!-- Nombre e imagen del poke -->
        <div
            class="mx-[1rem] p-[5rem] flex flex-col justify-center items-center bg-red-50 border-solid border-2 border-slate-300 rounded-full">
            <p class="font-bold text-4xl p-[1rem] mb-[5rem]">{{ nombrePokemon }}</p>
            <img :src="imagenPokemon" alt="">
        </div>
        <!-- Estadisticas -->
        <div class="w-full m-[1rem]">
            <p class=" flex felx-row justify-center font-bold text-4xl border-solid border-2 rounded-full bg-green-200">
                Estadisticas</p>
            <div class="bg-green-50 my-[2rem] p-[2rem]">
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. In obcaecati aliquid quisquam earum perferendis
                    deleniti omnis commodi porro magni accusamus, alias tempora. Numquam voluptatum rem ducimus sed, ex quia
                    asperiores!</p>
            </div>

        </div>

    </div>
</template>
<script>
export default {
    name: "pokemon",
    data() {
        return {
            nombrePokemon: $nuxt.$route.params.segundaPantalla,
            imagenPokemon: $nuxt.$route.query.imagen

        }
    },
    methods: {
        async info() {
            let { data } = await this.$axios.get(`pokemon/${this.nombrePokemon}/`)
            console.log(data);
        }
    },
    mounted() {
        console.log(this.$route)
        this.info()
    }
}</script>
