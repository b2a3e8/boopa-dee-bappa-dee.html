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
  // @ is an alias to /src
  import Navbar from '@/components/Navbar.vue'

  export default {
    components: {
      Navbar,
    }
  }
</script>

<!--<style>
</style>-->

<style lang="scss">
  // Set your colors
  $primary: #000045;
  $info: #DCDCDC;
  $warning: #FFCC11;
  $link: #EE9A00;

  // Import Bulma's core
  @import "~bulma/sass/utilities/_all";

  // Import Bulma and Buefy styles
  @import "~bulma";
  @import "~buefy/src/scss/buefy";
</style>
