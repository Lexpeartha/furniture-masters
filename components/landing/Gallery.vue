<template>
  <section class="bg-lightseagreen-50">
    <div class="container px-5 pt-6 pb-12 mx-auto">
      <div class="flex flex-col text-center w-full mb-20">
        <h1 class="sm:text-3xl text-2xl font-bold mb-4 text-brand">
          One of the biggest furniture selections in the world
        </h1>
        <p class="w-2/3 mx-auto leading-relaxed text-base text-chocolate-600">
          Whichever type of furniture you like, we have it. With our
          cooperation, we can make your dream house in no time!
        </p>
      </div>
      <div class="md:flex">
        <div
          v-for="(furItem, furIndex) in furnitureItems"
          :key="furIndex"
          class="lg:w-1/3 sm:w-1/2 mx-auto w-4/5 p-4"
        >
          <div class="flex relative">
            <img
              :alt="furItem.alt"
              class="absolute inset-0 w-full h-full object-cover object-center"
              :src="furItem.image"
            />
            <div
              class="px-4 py-8 relative z-10 w-full border-4 border-chocolate-200 bg-lightseagreen-50 transition-opacity duration-300 opacity-0 hover:opacity-100"
            >
              <h2 class="tracking-wide text-sm font-medium text-brand mb-1">
                {{ furItem.subtitle }}
              </h2>
              <h1 class="text-lg font-medium text-chocolate-800 mb-3">
                {{ furItem.title }}
              </h1>
              <p class="leading-relaxed text-chocolate-600">
                {{ furItem.content }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Gallery',
  data() {
    return {
      furnitureItems: [
        {
          subtitle: 'All types of chairs',
          title: 'Perfect combinations for all houses',
          image: 'https://bit.ly/3p8tjBl',
          alt: 'Gallery photo',
          content:
            'Our chairs here are not just for sitting, but for admiring and looking too!',
        },
        {
          subtitle: 'All types of kitchens',
          title: 'Be surrounded by beatiful furniture',
          image: 'https://bit.ly/38BuraX',
          alt: 'Gallery photo',
          content: `It's always awesome experience to eat in the place with just as awesome looks`,
        },
        {
          subtitle: 'All types of living-rooms',
          title: 'Relax with style and comfort',
          image: 'https://bit.ly/38pjzwo',
          alt: 'Gallery photo',
          content: `Forget all discomforts of life and chill in this soon to be your's living-room`,
        },
      ],
    }
  },
}
</script>

<style scoped></style>
