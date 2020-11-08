<template>
  <div>
    <Alert v-show="alert" @dismissed="dismissAlert" />
    <Navigation />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'DefaultLayout',
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
