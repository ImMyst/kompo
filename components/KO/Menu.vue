<template>
  <div
    class="flex justify-between items-center py-4 px-6 md:py-8 md:px-16 lg:px-36 xl:px-80"
  >
    <NuxtLink class="flex space-x-4" to="/">
      <img
        src="~/assets/icons/kompot-logo.svg"
        alt="Kompot"
        class="w-12 md:w-14 sm:-mt-1 md:-mt-2"
      />
      <h2 class="hidden sm:block main-title text-4xl">Kompot</h2>
    </NuxtLink>
    <div class="flex justify-end space-x-4">
      <NuxtLink
        v-for="(menuItem, id) in menuItems"
        :key="id"
        :to="menuItem.link"
        class="font-medium text-gray-500 hover:text-gray-900 md:text-lg"
      >
        {{ menuItem.label }}
      </NuxtLink>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data() {
    return {
      menuItems: [
        {
          label: 'Documentation',
          link: '/docs',
        },
      ],
    }
  },
})
</script>
