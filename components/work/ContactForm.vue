<template>
  <section class="relative">
    <div class="container px-5 py-24 mx-auto">
      <div class="flex flex-col text-center w-full mb-12">
        <h1 class="sm:text-3xl text-2xl font-medium mb-4 text-brand">
          Contact us
        </h1>
        <p
          class="lg:w-3/5 mx-auto text-left leading-relaxed text-base text-chocolate-600"
        >
          We like passionate and caring co-workers who have the same idea of
          creating better and more beatiful world, one piece of furniture at the
          time. Does that sound like you?
        </p>
      </div>
      <div class="lg:w-1/2 md:w-2/3 mx-auto">
        <div class="flex flex-wrap -m-2">
          <div class="p-2 w-1/2">
            <div class="relative">
              <label for="name" class="leading-7 text-sm text-brand opacity-75"
                >Name</label
              >
              <input
                id="name"
                type="text"
                name="name"
                class="w-full bg-opacity-50 bg-lightseagreen-50 border-brand focus:border-chocolate-600 text-chocolate-600 rounded-md border text-base outline-none py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
              />
            </div>
          </div>
          <div class="p-2 w-1/2">
            <div class="relative">
              <label for="email" class="leading-7 text-brand opacity-75"
                >Email</label
              >
              <input
                id="email"
                type="email"
                name="email"
                class="w-full bg-opacity-50 bg-lightseagreen-50 border-brand focus:border-chocolate-600 text-chocolate-600 border rounded-md text-base outline-none py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
              />
            </div>
          </div>
          <div class="p-2 w-full">
            <div class="relative">
              <label
                for="message"
                class="leading-7 text-sm text-brand opacity-75"
                >Message</label
              >
              <textarea
                id="message"
                name="message"
                class="w-full bg-opacity-50 bg-lightseagreen-50 border-brand focus:border-chocolate-600 text-chocolate-600 border rounded-md h-32 text-base outline-none py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out"
              ></textarea>
            </div>
          </div>
          <div class="p-2 w-full">
            <button
              class="flex mx-auto transition-opacity duration-300 text-lightseagreen-50 opacity-75 hover:opacity-100 bg-brand border-0 py-2 px-6 focus:outline-none rounded text-lg"
            >
              Submit
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ContactForm',
}
</script>

<style scoped></style>
