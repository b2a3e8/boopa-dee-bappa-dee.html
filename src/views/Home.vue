<template>
  <div class="home">

    <!--<h1 class="title">Translate ASCII to Boopa-dee Bappa-dee</h1>-->

    <div class="tabs">
      <ul>
        <li class="is-active"><a>ASCII to Boopa-dee</a></li>
        <li><a>Boopa-dee to ASCII</a></li>
      </ul>
    </div>

    <div class="columns is-desktop">
      <div class="column">
        <textarea class="textarea has-fixed-size is-shadowless is-info" placeholder="Type or paste text" rows="11"></textarea>
      </div>
      <div class="column is-narrow">
        <i class="fas fa-chevron-right" style="margin-top: 130px; color: #BABABA;"></i>
      </div>
      <div class="column">
        <textarea class="textarea has-fixed-size is-shadowless is-info" readonly rows="11"></textarea>
      </div>
    </div>

    <!--
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    -->
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
  }
}
</script>
