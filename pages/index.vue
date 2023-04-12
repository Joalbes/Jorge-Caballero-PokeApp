<template>
  <div class="h-screen">

    <div class="flex justify-center items-center py[1%]">
      <p class="text-6xl font-bold">PokeDEx</p>
    </div>

    <div>
      <input type="text" class="border-solid border-2 border-green-100 bg-green-50 mt-[2%]">
    </div>

    <div class="my-[2%] flex flex-wrap px-[5%] h-[80%]">
      <Card v-for="i in posts" :key="i.name" :nombre="i.name" :url="i.url" class="mx-[0.5%] my-[0.5%]"></Card>
    </div>

  </div>
</template>

<script>
import { log } from 'console';

export default {
  data() {
    return {
      posts: []
    };
  },
  mounted() {
    this.getInfo()
  },
  methods: {
    async getInfo() {
      const { data } = await this.$axios.get('pokemon')
      this.posts = data.results
      console.log(this.posts)
    },

    async getImage(){
      const {data1} = await this.$axios.get('pokemon')
      for (let index = 0; index < array.length; index++) {
                
      }

    }
  }
}
</script>
<style></style>
