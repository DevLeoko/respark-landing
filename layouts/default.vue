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
@import url('https://fonts.googleapis.com/css2?family=Sofia+Sans:wght@300;400;500;600;700&display=swap');

body {
  background-image: radial-gradient(at 50% 50%, rgba(89, 152, 219, 0.4) 0%, rgba(255, 255, 255, 0) 70%, rgba(228, 234, 238, 0) 100%);
  background-color: #edf3f5;
  font-family: 'Sofia Sans', sans-serif;
  background-size: 300% 300%;
  background-position: 40% 30%;
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
