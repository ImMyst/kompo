<template>
  <div class="pt-16 lg:pt-32 mb-auto">
    <h1
      class="text-4xl md:text-6xl lg:text-7xl main-title md:w-full lg:w-full xl:w-11/12"
    >
      Reusable and Responsive
      <span class="text-[#23b6d4]">Tailwind</span> Components for
      <span class="text-[#3fb27f]">Vue</span>
    </h1>
    <p
      class="text-lg text-gray-600 font-medium mt-8 leading-relaxed md:text-xl md:leading-relaxed sm:w-4/6 md:w-5/6 lg:w-5/6"
    >
      Kompot is a components library made by
      <a
        href="https://github.com/ImMyst"
        target="_blank"
        class="text-black font-bold underline-gradient"
        >Titouan G.</a
      >
      originally as a side project to facilitate and accelerate the development
      of UI and website. Feel free to take a look and add more components 😉 !
    </p>
    <div class="mt-12 md:mt-16 flex">
      <KOButton route="/docs" dlc="mr-3 lg:mr-4">Documentation</KOButton>
      <KOButton
        destination="https://github.com/ImMyst/kompot"
        :icon="githubIcon"
        light
      >
        Github
      </KOButton>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      githubIcon:
        'data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij48cGF0aCBkPSJNMTIgMGMtNi42MjYgMC0xMiA1LjM3My0xMiAxMiAwIDUuMzAyIDMuNDM4IDkuOCA4LjIwNyAxMS4zODcuNTk5LjExMS43OTMtLjI2MS43OTMtLjU3N3YtMi4yMzRjLTMuMzM4LjcyNi00LjAzMy0xLjQxNi00LjAzMy0xLjQxNi0uNTQ2LTEuMzg3LTEuMzMzLTEuNzU2LTEuMzMzLTEuNzU2LTEuMDg5LS43NDUuMDgzLS43MjkuMDgzLS43MjkgMS4yMDUuMDg0IDEuODM5IDEuMjM3IDEuODM5IDEuMjM3IDEuMDcgMS44MzQgMi44MDcgMS4zMDQgMy40OTIuOTk3LjEwNy0uNzc1LjQxOC0xLjMwNS43NjItMS42MDQtMi42NjUtLjMwNS01LjQ2Ny0xLjMzNC01LjQ2Ny01LjkzMSAwLTEuMzExLjQ2OS0yLjM4MSAxLjIzNi0zLjIyMS0uMTI0LS4zMDMtLjUzNS0xLjUyNC4xMTctMy4xNzYgMCAwIDEuMDA4LS4zMjIgMy4zMDEgMS4yMy45NTctLjI2NiAxLjk4My0uMzk5IDMuMDAzLS40MDQgMS4wMi4wMDUgMi4wNDcuMTM4IDMuMDA2LjQwNCAyLjI5MS0xLjU1MiAzLjI5Ny0xLjIzIDMuMjk3LTEuMjMuNjUzIDEuNjUzLjI0MiAyLjg3NC4xMTggMy4xNzYuNzcuODQgMS4yMzUgMS45MTEgMS4yMzUgMy4yMjEgMCA0LjYwOS0yLjgwNyA1LjYyNC01LjQ3OSA1LjkyMS40My4zNzIuODIzIDEuMTAyLjgyMyAyLjIyMnYzLjI5M2MwIC4zMTkuMTkyLjY5NC44MDEuNTc2IDQuNzY1LTEuNTg5IDguMTk5LTYuMDg2IDguMTk5LTExLjM4NiAwLTYuNjI3LTUuMzczLTEyLTEyLTEyeiIvPjwvc3ZnPg==',
    }
  },
})
</script>

<style></style>
