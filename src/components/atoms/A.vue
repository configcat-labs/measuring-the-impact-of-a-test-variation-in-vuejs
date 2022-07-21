<script>
export default {
  setup() {
    
  },
  props: {
    path: String,
  }
}
</script>

<template>
  <router-link :to="path" class="block py-2 pr-4 pl-3 text-blue-700 rounded md:bg-transparent my-1 md:p-0 dark:text-white" aria-current="page">
    <slot />
  </router-link>
</template>