<template>
  <div class="home">

    <div class="tabs">
      <ul>
        <li class="is-active"><a>ASCII to Boopa-dee</a></li>
        <li><a>Boopa-dee to ASCII</a></li>
      </ul>
    </div>

    <div class="columns is-desktop is-vcentered">
      <div class="column">
        <textarea class="textarea has-fixed-size is-shadowless is-info" placeholder="Type or paste text" rows="11"></textarea>
      </div>
      <!--<div class="column is-narrow" style="position: relative;">
        <i class="fas fa-chevron-right" style="color: #BABABA; position: absolute; top: 50%; left: 35%;"></i>
      </div>-->
      <div class="column is-narrow is-hidden-touch">
        <i class="fas fa-chevron-right" style="color: #BABABA;"></i>
      </div>
      <div class="column">
        <textarea class="textarea has-fixed-size is-shadowless is-info" readonly rows="11"></textarea>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'home',
  components: {
  }
}
</script>
