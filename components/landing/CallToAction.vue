<template>
  <section
    class="antialiased md:px-4 px-20 w-full bg-lightseagreen-50 text-center py-8"
  >
    <div class="container mx-auto max-w-3xl py-8">
      <h3 class="text-3xl font-bold text-brand">
        Join thousands of other happy customers today!
      </h3>
      <p class="mt-12 mb-2 text-chocolate-600">
        Join the fun just by giving us your email, we will contact you very
        shortly to predetermine our meetings where we will discuss both sides'
        visions of your new indoors
      </p>
      <div class="my-8 md:flex">
        <input
          type="email"
          class="w-full bg-lightseagreen-50 rounded border border-brand focus:border-chocolate-600 text-base outline-none text-chocolate-600 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
          name="email"
          placeholder="Enter your email"
        />
        <button
          class="inline-flex mt-8 md:mt-0 transition-opacity duration-300 text-lightseagreen-50 opacity-75 hover:opacity-100 bg-brand border-0 md:ml-12 py-2 px-6 focus:outline-none rounded text-lg"
        >
          Subscribe
        </button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CTA',
}
</script>

<style scoped></style>
