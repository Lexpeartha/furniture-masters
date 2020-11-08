<template>
  <div>
    <Alert v-show="alert" @dismissed="dismissAlert" />
    <Navigation />
    <Nuxt />
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
