<template>
  <div class="bg-[#18181b] text-gray-100 w-full lg:pt-[60px] p-14">
    <Container>
      <div class="w-auto h-auto bg-[#27272a] rounded-md shadow-md overflow-hidden">
        <div class="md:flex">
          <div class="md:flex-shrink-0">
            <nuxt-img
              sizes="sm:212px lg:350px"
              src="/images/avatars/AvatarMe.png"
              alt=""
              class="w-full h-full aspect-w-1 aspect-h-1 p-4"
            />
          </div>
          <div class="p-12">
            <div class="uppercase tracking-wide text-sm text-indigo-500 font-semibold mt-2"> {{ data.main.about }} </div>
            <p class="mt-4 text-xl lg:text-2xl text-[#fafafa]"> {{ data.main.name }} </p>
            <p class="mt-4 text-[#f4f4f5]"> {{ data.main.occupation }} </p>
            <p class="mt-4 text-lg text-[#a1a1aa]"> {{ data.main.bio }} </p>
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
  name: 'About',
  components: {
    Container,
  },
  data() {
    return {
      data,
    }
  }
}
</script>
