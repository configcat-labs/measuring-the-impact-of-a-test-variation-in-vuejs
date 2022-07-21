<script>

// Imports
import SiteLayout from './views/layout/SiteLayout.vue'

export default {
  setup() {
    
  },
  data() {
    return {
      navigationItems: [
        {
          path: '/',
          label: 'Home',
        },
        {
          path: '/',
          label: 'Loans',
        },
        {
          path: '/',
          label: 'Services',
        },
        {
          path: '/',
          label: 'Legal',
        },
        {
          path: '/',
          label: 'Home',
        },
      ]
    }
  },
  components: {
    SiteLayout,
  }
}
</script>

<template>
  <SiteLayout :navigationItems="navigationItems">
    <router-view></router-view>
  </SiteLayout>
</template>