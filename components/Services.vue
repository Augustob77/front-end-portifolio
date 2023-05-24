<template>
  <div class="bg-[#18181b] text-gray-100 w-full lg:pt-[40] p-14">
    <h3 class="text-center text-4xl py-6"> Conhecimentos <span class="text-[#5b21b6]"> . </span> </h3>
    <Container>
      <div class="bg-[#0a0a0a] w-auto h-auto rounded-md shadow-md p-8">
        <div class="flex justify-between">
          <div class="w-1/3 border border-purple-600 rounded-md m-4">
            <nuxt-img
              sizes="sm:212px lg:350px"
              src="/images/avatars/AvatarMe.png"
              alt=""
              class="w-full h-full aspect-w-1 aspect-h-1 p-1"
            />
          </div>

          <div class="w-1/3 border border-purple-600 rounded-md m-4">
            <nuxt-img
              sizes="sm:212px lg:350px"
              src="/images/avatars/AvatarMe.png"
              alt=""
              class="w-full h-full aspect-w-1 aspect-h-1 p-1"
            />
          </div>
          
          <div class="w-1/3 border border-purple-600 rounded-md m-4">
            <nuxt-img
              sizes="sm:212px lg:350px"
              src="/images/avatars/AvatarMe.png"
              alt=""
              class="w-full h-full aspect-w-1 aspect-h-1 p-1"
            />
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

  