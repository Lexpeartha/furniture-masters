<template>
  <header class="text-chocolate-600 bg-lightseagreen-50 body-font">
    <div
      class="container mx-auto sticky flex flex-wrap md:p-4 px-6 py-4 flex-row justify-between md:items-center"
    >
      <nuxt-link to="/" class="flex font-medium items-center mb-0">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          class="w-10 h-10 p-2 text-lightseagreen-50 bg-brand rounded-full"
          viewBox="0 0 24 24"
        >
          <path
            d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5"
          ></path>
        </svg>
        <span class="ml-3 text-xl text-chocolate-600">Furniture Masters</span>
      </nuxt-link>
      <nav class="flex flex-wrap items-center text-base justify-center">
        <nuxt-link
          v-for="(navItem, navIndex) in navItems"
          :key="navIndex"
          :to="navItem.route"
          class="mr-5 hover:text-brand hidden md:block cursor-pointer"
          >{{ navItem.name }}</nuxt-link
        >
      </nav>

      <div class="relative mt-2">
        <button
          id="hamburger"
          class="md:hidden block bg-transparent focus:outline-none"
          @click="hamburgerOnClick"
          @mouseenter="isNavExpanded = true"
        >
          <transition mode="out-in" name="switch">
            <svg
              v-if="isNavExpanded"
              key="x"
              xmlns="http://www.w3.org/2000/svg"
              width="30"
              height="30"
              viewBox="0 0 24 24"
            >
              <path
                fill="#6CD400"
                d="M24 20.188l-8.315-8.209 8.2-8.282-3.697-3.697-8.212 8.318-8.31-8.203-3.666 3.666 8.321 8.24-8.206 8.313 3.666 3.666 8.237-8.318 8.285 8.203z"
              />
            </svg>
            <svg v-else key="ham" viewBox="0 0 18 15" width="30" height="30">
              <path
                fill="#6CD400"
                d="M18,1.484c0,0.82-0.665,1.484-1.484,1.484H1.484C0.665,2.969,0,2.304,0,1.484l0,0C0,0.665,0.665,0,1.484,0 h15.031C17.335,0,18,0.665,18,1.484L18,1.484z"
              />
              <path
                fill="#6CD400"
                d="M18,7.516C18,8.335,17.335,9,16.516,9H1.484C0.665,9,0,8.335,0,7.516l0,0c0-0.82,0.665-1.484,1.484-1.484 h15.031C17.335,6.031,18,6.696,18,7.516L18,7.516z"
              />
              <path
                fill="#6CD400"
                d="M18,13.516C18,14.335,17.335,15,16.516,15H1.484C0.665,15,0,14.335,0,13.516l0,0 c0-0.82,0.665-1.484,1.484-1.484h15.031C17.335,12.031,18,12.696,18,13.516L18,13.516z"
              />
            </svg>
          </transition>
        </button>

        <transition name="slide" tag="div">
          <div
            v-if="isNavExpanded"
            id="mobileNav"
            class="absolute py-3 px-2 w-32 md:hidden bg-lightseagreen-50 text-chocolate-600 right-0 flex flex-col"
            @mouseleave="isNavExpanded = false"
          >
            <nuxt-link
              v-for="(navItem, navIndex) in navItems"
              :key="navIndex"
              :to="navItem.route"
              class="nav-link mr-5 hover:text-brand cursor-pointer"
              @click.native="isNavExpanded = false"
              >{{ navItem.name }}</nuxt-link
            >
          </div>
        </transition>
      </div>

      <button
        class="items-center hidden opacity-75 hover:opacity-100 md:block bg-brand text-lightseagreen-50 border-0 py-1 px-3 focus:outline-none rounded text-base"
      >
        Let us help you!
      </button>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Navigation',
  data() {
    return {
      isNavExpanded: false,
      navItems: [
        {
          name: 'Home',
          route: '/',
        },
        {
          name: 'About us',
          route: '/about',
        },
        {
          name: 'Work with us',
          route: '/work',
        },
      ],
    }
  },
  methods: {
    hamburgerOnClick() {
      this.isNavExpanded = !this.isNavExpanded
    },
    beforeEnter(element) {},
    enter(element, next) {},
    leave(element, next) {},
  },
}
</script>

<style scoped>
.switch-enter-active {
  animation: switch-in 350ms;
}

.switch-leave-active {
  animation: switch-in 350ms reverse;
}

.slide-enter-active {
  animation: slide-in 400ms;
}

.slide-leave-active {
  animation: slide-in 400ms reverse;
}

@keyframes switch-in {
  0% {
    opacity: 0%;
  }
  50% {
    opacity: 50%;
  }
  100% {
    opacity: 100%;
  }
}

@keyframes slide-in {
  0% {
    opacity: 0%;
    transform: translateX(30%);
  }
  50% {
    opacity: 50%;
    transform: translateX(15%);
  }
  100% {
    opacity: 100%;
    transform: translateX(0%);
  }
}
</style>
