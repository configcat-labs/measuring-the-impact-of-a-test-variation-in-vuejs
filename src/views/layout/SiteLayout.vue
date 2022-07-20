<script>

// Import
import Navbar from '../../components/shared/Navbar.vue'
import Footer from '../../components/shared/Footer.vue'

export default {
  setup() {
    
  },
  components: {
    Navbar,
    Footer,
  }
}
</script>

<template>
  <div>
    <!-- Navbar -->
    <Navbar />

    <main>
      <slot />
    </main>

    <!-- Footer -->
    <Footer />
  </div>
</template>