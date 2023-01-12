<template>
  <div class="flex flex-col w-full min-h-screen justify-center items-center p-4">
    <img src="/images/logo.svg" alt="Respark logo" class="w-64 md:w-lg mt-auto" />
    <div class="max-w-xl">
      <slot />
    </div>
    <div class="self-end mt-auto flex">

      <router-link to="impressum">Imprint</router-link>
      <router-link to="privacy-policy" class="ml-3">Privacy policy</router-link>
    </div>
  </div>
</template>

<script lang='ts'>
import { defineComponent } from 'vue';

export default defineComponent({
  data() {
    return {};
  }
});
</script>

<style>
/* sofia-sans-300 - latin */
@font-face {
  font-family: 'Sofia Sans';
  font-style: normal;
  font-weight: 300;
  src: local(''),
    url('/fonts/sofia-sans-v10-latin-300.woff2') format('woff2'),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/sofia-sans-v10-latin-300.woff') format('woff');
  /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* sofia-sans-regular - latin */
@font-face {
  font-family: 'Sofia Sans';
  font-style: normal;
  font-weight: 400;
  src: local(''),
    url('/fonts/sofia-sans-v10-latin-regular.woff2') format('woff2'),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/sofia-sans-v10-latin-regular.woff') format('woff');
  /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* sofia-sans-500 - latin */
@font-face {
  font-family: 'Sofia Sans';
  font-style: normal;
  font-weight: 500;
  src: local(''),
    url('/fonts/sofia-sans-v10-latin-500.woff2') format('woff2'),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/sofia-sans-v10-latin-500.woff') format('woff');
  /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* sofia-sans-600 - latin */
@font-face {
  font-family: 'Sofia Sans';
  font-style: normal;
  font-weight: 600;
  src: local(''),
    url('/fonts/sofia-sans-v10-latin-600.woff2') format('woff2'),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/sofia-sans-v10-latin-600.woff') format('woff');
  /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* sofia-sans-700 - latin */
@font-face {
  font-family: 'Sofia Sans';
  font-style: normal;
  font-weight: 700;
  src: local(''),
    url('/fonts/sofia-sans-v10-latin-700.woff2') format('woff2'),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
    url('/fonts/sofia-sans-v10-latin-700.woff') format('woff');
  /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

body {
  background-image: radial-gradient(at 50% 50%, rgba(89, 152, 219, 0.4) 0%, rgba(255, 255, 255, 0) 70%, rgba(228, 234, 238, 0) 100%);
  background-color: #edf3f5;
  font-family: 'Sofia Sans', sans-serif;
  background-size: 200% 200%;
  background-position: 20% 80%;
  animation: background-sweep 60s ease infinite;
}

@keyframes background-sweep {
  0% {
    background-position: 20% 80%;
  }

  40% {
    background-position: 80% 90%;
  }

  60% {
    background-position: 70% 30%;
  }

  80% {
    background-position: 20% 10%;
  }

  100% {
    background-position: 20% 80%;
  }
}
</style>
