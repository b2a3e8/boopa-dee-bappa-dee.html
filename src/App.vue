<template>
  <div id="app">
    <Navbar />
    <div class="container">
      <router-view/>
    </div>
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

<style>
</style>
