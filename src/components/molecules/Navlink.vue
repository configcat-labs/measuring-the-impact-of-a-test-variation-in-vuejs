<script>

// Imports
import A from '@/components/atoms/A.vue';

export default {
  setup() {
    
  },
  components: {
    A,
  },
  props: {
    navigationItem: Object,
  }
}
</script>

<template>
  <li>
    <A :path="navigationItem.path">{{ navigationItem.label }}</A>
  </li>
</template>