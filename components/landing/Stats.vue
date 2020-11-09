<template>
  <section class="text-gray-700 py-20 bg-lightseagreen-50">
    <h1 class="sm:text-3xl text-2xl font-bold text-brand text-center">
      Our success in numbers
    </h1>
    <div class="container px-6 py-20 mx-auto">
      <div class="flex flex-wrap -m-4 text-center">
        <div
          v-for="(stat, statIndex) in stats"
          :key="statIndex"
          class="p-4 md:w-1/3 w-full"
        >
          <h2 class="title-font font-medium sm:text-4xl text-3xl text-gray-900">
            {{ stat.value }}
          </h2>
          <p class="leading-relaxed">{{ stat.name }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Stats',
  data() {
    return {
      stats: [
        {
          name: 'Daily users',
          value: '6.9K',
        },
        {
          name: '5-star reviews',
          value: '10000+',
        },
        {
          name: 'Products in our stores',
          value: 'over 2000',
        },
      ],
    }
  },
}
</script>

<style scoped></style>
