<template>
  <escape-keypad :text-done="textDone" :relative-keyboard-coords="[17,18,65,73]" skin="/static/keypad-skins/keypad3.png"
                 class="main-keypad3" combination-hash="$2a$04$xeJX0bMdGgMWfhMX.x.Im.xNTB/JDtipRqHuzhHixXJKWHEnRg/pm"
                 :number-of-digits="4"></escape-keypad>
</template>
<style>
  .main-keypad3 {
    width: 100%;
  }


  .main-keypad3 .keypad input {
    position: relative;
    background-color: #000;
    color: #fff;
    border: solid 1px #fff;
  }

  .main-keypad3 .keypad img {
    max-width: 100%;
  }

  .overpose {
    position:relative;
    left: -220px;
    -webkit-animation: flickerAnimation 1s infinite;
    -moz-animation: flickerAnimation 1s infinite;
    -o-animation: flickerAnimation 1s infinite;
    animation: flickerAnimation 1s infinite;
  }

  .imagesEnd {
    width: 249px !important;
    margin: auto;
    white-space:nowrap;
  }

  @keyframes flickerAnimation {
    0%   { opacity:1; }
    50%  { opacity:0; }
    100% { opacity:1; }
  }
  @-o-keyframes flickerAnimation{
    0%   { opacity:1; }
    50%  { opacity:0; }
    100% { opacity:1; }
  }
  @-moz-keyframes flickerAnimation{
    0%   { opacity:1; }
    50%  { opacity:0; }
    100% { opacity:1; }
  }
  @-webkit-keyframes flickerAnimation{
    0%   { opacity:1; }
    50%  { opacity:0; }
    100% { opacity:1; }
  }


  @media screen and (orientation:portrait) {
    .main-keypad3 .under-door p {
      font-size: 6vw;
    }
  }

  @media screen and (orientation:landscape) {
    .main-keypad3 .under-door p {
      font-size: 6vh;
      width: 80%;
      margin-left: auto;
      margin-right: auto;
    }
  }
</style>
<script>
  import EscapeKeypad from '../components/Keypad.vue'

  export default {
    components: {
      EscapeKeypad
    },
    data () {
      return {
        textDone: '<p>¡Enhorabuena!</p>' +
        '<p>¡Habéis evitado una catástrofe gracias a vuestras habilidades! Además,  el código ha redirigido el misil hacia el líder Parayerista, eliminando la amenaza para siempre.</p>' +
        '<p class="imagesEnd"><img src="/static/the-end/lo-malo.jpg"/><img src="/static/the-end/bomb.png" class="overpose"/></p>' +
        '<p><b>¡Felicidades!</b></p>'
      }
    }
  }
</script>

