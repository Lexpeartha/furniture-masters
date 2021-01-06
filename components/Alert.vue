<template>
  <section id="alert" class="bg-lightseagreen-200 text-chocolate-800 py-4 px-6">
    <div class="container items-center flex max-w-2xl m-auto leading-none">
      <span
        class="flex rounded-full bg-lightseagreen-50 uppercase px-2 py-1 text-xs font-bold mr-3"
        >New!</span
      >
      <span class="mx-auto"
        >New Furnitures! New products have been added recently, check them
        out!</span
      >
      <span
        class="text-sm cursor-pointer hover:text-chocolate-900"
        @click="dismissModal"
        >x</span
      >
    </div>
  </section>
</template>

<script>
export default {
  name: 'Alert',
  methods: {
    dismissModal() {
      this.$emit('dismissed')
    },
  },
}
</script>

<style scoped></style>
