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
          label: 'Home'
        }
      ]
    }
  },
  components: {
    SiteLayout,
  }
}
</script>

<template>
  <SiteLayout>
    <router-view></router-view>
  </SiteLayout>
</template>