<template>
  <div class="bg-[#0a0a0a] text-gray-100 w-full pt-[70px] lg:pt-[120px]">
    <Container>
      <div class="flex flex-col-reverse lg:flex-row pb-[154px] lg:pb-[206px]">
        <div class="header__content w-full lg:w-8/12 text-center lg:text-left">
          <h1 class="text-xl lg:text-6xl font-sans mt-[28px] lg:mt-none">
            {{ data.main.name }}
          </h1>

          <h2 class="text-2xl lg:text-1xl mt-[20px] lg:mt-[30px]">
            {{ data.main.occupation }}
          </h2>

          <a href="https://www.instagram.com/augustob77/" class="inline-block text-xl lg:text-2xl bg-[#5b21b6] text-[#f5f3ff] py-2 lg:py-4 px-[90px] lg:px-10 rounded mt-[40px] hover:bg-[#2e1065] hover:text-[#6d28d9]">
            Instagram
          </a>
        </div>

        <div class="w-full lg:w-4/12">
          <div class="overflow-hidden w-8/12 md:w-4/12 lg:w-full mx-auto lg:mx-[0px]">
            <nuxt-img
              sizes="sm:212px lg:350px"
              src="/images/avatars/avatar.png"
              alt=""
              class="w-full h-full aspect-w-1 aspect-h-1"
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
  name: 'Header',
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
