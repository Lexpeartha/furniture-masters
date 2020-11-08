<template>
  <section class="text-gray-700 body-font">
    <div
      class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center"
    >
      <div
        class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"
      >
        <h1
          class="title-font sm:text-4xl text-3xl mb-4 font-medium text-gray-900"
        >
          Get your dream furniture, now
        </h1>
        <p class="mb-8 leading-relaxed">
          We work with you to design and choose perfect furniture for your home.
          Our catalog of beatiful furniture is huge, and we guarantee to find
          the one that suits you perfectly.
        </p>
        <div class="flex w-full md:justify-start justify-center items-end">
          <div class="relative mr-4 md:w-full lg:w-full xl:w-1/2 w-2/4">
            <label for="hero-field" class="leading-7 text-sm text-gray-600"
              >Placeholder</label
            >
            <input
              id="hero-field"
              type="text"
              name="hero-field"
              class="w-full bg-gray-100 rounded border border-gray-300 focus:border-indigo-500 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
            />
          </div>
          <button
            class="inline-flex text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg"
          >
            Button
          </button>
        </div>
        <p class="text-sm mt-2 text-gray-500 mb-8 w-full">
          Neutra shabby chic ramps, viral fixie.
        </p>
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
