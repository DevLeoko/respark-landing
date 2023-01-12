<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup() {
    return {
      contactMethods: [
        { name: 'mail', link: 'mailto:lets@respark.dev', text: 'lets@respark.dev' },
      ]
    }
  },
})
</script>

<template>
  <h1 class="text-3xl font-bold mt-5">Innovative solutions, ignited by Respark</h1>
  <h2 class="text-xl my-16">
    The web presence is still under development - check back in later!
  </h2>
  <article class="flex flex-col items-center">
    <h3>Can't wait? Get in touch:</h3>
    <ul>
      <li v-for="contact in contactMethods">
        <a :href="contact.link" target="_blank" class="flex">
          <img :src="`/images/${contact.name}.svg`" :alt="contact.name" class="h-5 mr-1"> {{
              contact.text
          }}
        </a>
      </li>
    </ul>
  </article>
</template>
