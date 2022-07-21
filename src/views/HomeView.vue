<script>

// Imports
import Banner from '@/components/molecules/Banner.vue';
import SocialProof from '@/components/organisms/pages/home/SocialProof.vue';
import WhoWeAre from '@/components/organisms/pages/home/WhoWeAre.vue';

export default {
  setup() {
    
  },
  components: {
    Banner,
    SocialProof,
    WhoWeAre,
  }
}
</script>

<template>
  <div>
    <Banner />
    <SocialProof />
    <WhoWeAre />
  </div>
</template>
