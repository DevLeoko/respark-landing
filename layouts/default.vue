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
  background-image: radial-gradient(at 83% 12%, rgba(0, 133, 173, 0.3) 0%, rgba(255, 255, 255, 0) 90%, rgba(228, 234, 238, 0) 100%);
  background-color: #edf3f5;
  font-family: 'Sofia Sans', sans-serif;
}

/* body {
  background-image: radial-gradient(at 95% 2%, rgba(73, 141, 161, 0.3) 0%, rgb(16, 18, 19) 100%);
  background-color: #101213;
} */
</style>
