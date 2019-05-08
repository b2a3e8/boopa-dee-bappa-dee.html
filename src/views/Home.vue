<template>
  <div class="home">

    <div class="tabs">
      <ul>
        <li :class="{ 'is-active': (mode === 'ascii-to-boopa') }"><a @click="mode = 'ascii-to-boopa'; autoDetectMode = false;">ASCII to Boopa-dee</a></li> <!-- TODO trigger translating on click -->
        <li :class="{ 'is-active': (mode === 'boopa-to-ascii') }"><a @click="mode = 'boopa-to-ascii'; autoDetectMode = false;">Boopa-dee to ASCII</a></li> <!-- TODO trigger translating on click -->
      </ul>
    </div>

    <div class="columns is-desktop is-vcentered">
      <div class="column">
        <textarea v-model="input" @input="translate()" class="textarea has-fixed-size is-shadowless is-info" placeholder="Type or paste text" rows="11"></textarea>
      </div>
      <div class="column is-narrow is-hidden-touch">
        <i class="fas fa-chevron-right" style="color: #BABABA;"></i>
      </div>
      <div class="column">
        <textarea v-model="output" class="textarea has-fixed-size is-shadowless is-info" readonly rows="11"></textarea>
      </div>
    </div>

  </div>
</template>

<script>
import _ from 'lodash';
import boopadee from 'boopa-dee-bappa-dee.js';

export default {
  name: 'home',
  components: {
  },
  data() {
    return {
      autoDetectMode: true,
      mode: 'ascii-to-boopa',
      input: '',
      output: '',
    };
  },
  methods: {
    translate: async function () {
      // detect mode
      if (this.autoDetectMode) {
        if (this.input.match(/^(bappadee|boo|boopa|bappa|dee|boopadee|baa| )+/)) {
          this.mode = 'boopa-to-ascii';
        } else {
          this.mode = 'ascii-to-boopa';
        }
      }

      // translate
      if (this.mode === 'ascii-to-boopa') {
        this.output = await boopadee.encode(this.input);
      } else {
        try {
          this.output = await boopadee.decode(this.input);
        } catch (error) {
          console.log(error);
        }
      }
    },
  }
}
</script>
