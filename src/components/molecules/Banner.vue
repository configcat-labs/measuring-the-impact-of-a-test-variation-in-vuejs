<script>

// Import the amplitude configuration in this component.
import { ampli } from '../../ampli';

export default {
  setup() {
    // Initialize amplitude with the production environment
    ampli.load({ environment: 'production' });
  },
  methods: {
    handleLoanSignupClick() {
      // Log the event to amplitude when the loan signup button is clicked
      ampli.loanSignupClick();
    }
  }
}

</script>

<template>
  <section id="banner" class="bg-white dark:bg-gray-900">
      <div class="py-8 px-4 mx-auto max-w-screen-xl sm:py-16 lg:px-6">
          <div class="mx-auto max-w-screen-sm text-center">
              <!-- <h2 class="mb-4 text-4xl tracking-tight font-extrabold leading-tight text-gray-100 dark:text-white">Need a loan?</h2> -->
              <h2 class="mb-4 text-4xl tracking-tight font-extrabold leading-tight text-gray-100 dark:text-white">Get a loan immediately!</h2>
              <p class="mb-6 font-light text-gray-200 dark:text-gray-400 md:text-lg">Get instant approval at selective branches. Offer valid until September 2022.</p>
              <a @click="handleLoanSignupClick" href="#" class="text-white bg-blue-700 hover:bg-blue-800 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800">Claim my offer now!</a>
          </div>
      </div>
  </section>
</template>

<style scoped>
#banner {
  background-color: #663399;
}

</style>