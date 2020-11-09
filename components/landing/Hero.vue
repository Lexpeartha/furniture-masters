<template>
  <section class="text-gray-700 body-font">
    <div
      class="container mx-auto flex px-5 pt-24 pb-6 md:flex-row flex-col items-center"
    >
      <div
        class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"
      >
        <h1 class="sm:text-4xl text-3xl mb-4 font-bold text-brand">
          Get your dream furniture, now
        </h1>
        <p class="mb-8 leading-relaxed text-chocolate-600">
          We work with you to design and choose perfect furniture for your home.
          Our catalog of beatiful furniture is huge, and we guarantee to find
          the one that suits you perfectly.
        </p>
        <div class="flex w-full md:justify-start justify-center items-end">
          <div class="relative mr-4 md:w-full lg:w-full xl:w-1/2 w-2/4">
            <label
              for="hero-field"
              class="leading-7 text-sm text-brand opacity-75"
              >Place your email here so we can get in touch</label
            >
            <input
              id="hero-field"
              type="email"
              name="hero-field"
              class="w-full bg-lightseagreen-50 rounded border border-brand focus:border-chocolate-600 text-base outline-none text-chocolate-600 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
            />
          </div>
          <button
            class="inline-flex transition-opacity duration-300 text-lightseagreen-50 opacity-75 hover:opacity-100 bg-brand border-0 py-2 px-6 focus:outline-none rounded text-lg"
          >
            Submit
          </button>
        </div>
      </div>
      <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6">
        <img
          class="object-cover object-center shadow-lg rounded"
          alt="hero"
          src="https://bit.ly/3eDxyjh"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Features',
}
</script>

<style scoped></style>
