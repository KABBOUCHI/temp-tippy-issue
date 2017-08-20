<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view></router-view>
    <button class="btn"
            v-tippy
            data-distance="15"
            data-theme="light"
            data-animation="scale"
            data-arrowsize="big"
            data-interactive="true"
            data-animatefill="false"
            data-arrow="true"
            data-trigger="click"
            data-html="#comppopup">
                Popover Vue Component
    </button>
    <GoogleMaps style="visibility: hidden;" id="comppopup"></GoogleMaps>
  </div>
</template>

<script>
import GoogleMaps from './components/GoogleMaps.vue'

export default {
  name: 'app',
  components: {
    GoogleMaps
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
