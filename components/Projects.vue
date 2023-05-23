<template>
  <div class="bg-[#0a0a0a] text-gray-100 w-full lg:pt-[40] p-14">
    <h3 class="text-center text-4xl py-6"> Projetos <span class="text-[#5b21b6]"> . </span> </h3>
    <Container>
      <div class="w-auto h-auto rounded-md shadow-md p-8">
        <div class="flex justify-between">
          <div class="w-1/3 border border-red-600 rounded-md p-4 m-4">
            <h2 class="text-lg font-semibold"> {{ data.portfolio.projects[0].title }} </h2>
            <p class="text-[#a1a1aa]"> {{ data.portfolio.projects[0].description }} </p>
          </div>

          <div class="w-1/3 border border-blue-600 rounded-md p-4 m-4">
            <h2 class="text-lg font-semibold"> {{ data.portfolio.projects[1].title }} </h2>
            <p class="text-[#a1a1aa]"> {{ data.portfolio.projects[1].description }}  </p>
          </div>
          
          <div class="w-1/3 border border-green-600 rounded-md p-4 m-4">
            <h2 class="text-lg font-semibold"> {{ data.portfolio.projects[2].title }} </h2>
            <p class="text-[#a1a1aa]"> {{ data.portfolio.projects[2].description }}  </p>
          </div>
        </div>
      </div>
    </Container>
  </div>
</template>
  
  <script>
  import data from '../assets/api/data.json'
  import Container from './Container.vue'

  export default {
    name: 'Projects',
    components: {
    Container,
  },
    data() {
      return {
        data,
      };
    },
  };
  </script>

  