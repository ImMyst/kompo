<template>
  <div>
    <NuxtLink
      v-if="route"
      :to="route"
      :class="light ? 'btn-light' : 'btn-primary'"
    >
      <img v-if="icon" class="mr-2" :src="icon" alt="Button icon" />
      <slot />
    </NuxtLink>
    <a
      v-else
      :href="destination"
      :target="target"
      :class="light ? 'btn-light' : 'btn-primary'"
    >
      <img v-if="icon" class="mr-2" :src="icon" alt="Button icon" />
      <slot />
    </a>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  props: {
    route: {
      type: String,
      default: '',
    },
    destination: {
      type: String,
      default: '',
    },
    target: {
      type: String,
      default: '_blank',
    },
    light: {
      type: Boolean,
      default: false,
    },
    icon: {
      type: String,
      default: '',
    },
  },
})
</script>

<style lang="postcss" scoped>
.btn-primary {
  @apply flex text-gray-50 bg-gray-900 px-5 py-3 rounded-md font-bold shadow-md text-lg hover:bg-gray-700 hover:shadow-sm active:bg-gray-900 focus:ring-2;
}
.btn-light {
  @apply flex text-gray-900 px-5 py-3 font-bold text-lg hover:underline;
}
</style>
