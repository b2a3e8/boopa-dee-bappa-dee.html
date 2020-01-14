<template>
  <div id="app">
    <Navbar />
    <section class="section">
      <div class="container">
        <router-view/>
      </div>
    </section>
  </div>
</template>

<script>
  import Navbar from '@/components/Navbar.vue'

  export default {
    components: {
      Navbar,
    }
  }
</script>

<style lang="scss">
  // Set colors
  $primary: #000045;
  $info: #DCDCDC;
  $warning: #EE9A00;
  $link: #EE9A00;

  // Import Bulma's core
  @import "~bulma/sass/utilities/_all";

  // Import Bulma and Buefy styles
  @import "~bulma";
  @import "~buefy/src/scss/buefy";
</style>
