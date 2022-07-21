<script>

// Import
import Navbar from '../../components/shared/Navbar.vue'
import Main from '@/components/organisms/Main.vue'
import Footer from '../../components/shared/Footer.vue'

export default {
  setup() {
    
  },
  props: {
    navigationItems: Array,
  },
  components: {
    Navbar,
    Main,
    Footer,
  }
}
</script>

<template>
  <div>
    <!-- Navbar -->
    <div class="sticky top-0">
      <Navbar :navigationItems="navigationItems" />
    </div>

    <Main>
      <slot />
    </Main>

    <!-- Footer -->
    <Footer />
  </div>
</template>