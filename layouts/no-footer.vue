<template>
  <div>
    <transition> <Alert v-show="alert" @dismissed="dismissAlert" /></transition>

    <Navigation />
    <Nuxt />
  </div>
</template>

<script>
export default {
  name: 'NoFooter',
  data() {
    return {
      alert: true,
    }
  },
  methods: {
    dismissAlert() {
      this.alert = false
    },
  },
}
</script>
