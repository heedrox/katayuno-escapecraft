<template>
  <escape-keypad :text-done="textDone" :relative-keyboard-coords="[20,12,80,85]" skin="/static/keypad-skins/keypad1.png"
                 class="main-keypad" combination-hash="$2a$08$GnZouCpA1PtQ6MzfqkjnseGijHbkk7iCBvTiH3lCKXcte6N/xEh7O"></escape-keypad>
</template>
<style>
  .main-keypad {
    width: 100%;
  }

  .main-keypad .under-door p {
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }

  @media screen and (orientation:portrait) {
    .main-keypad .under-door p {
      font-size: 6vw;
    }
  }

  @media screen and (orientation:landscape) {
    .main-keypad .under-door p {
      font-size: 6vh;
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
        textDone: '<p><b>¡Enhorabuena!</b></p><p>Habéis demostrado ser buenos agentes.<br/>Sin embargo, ¡no parece que la bomba se haya detenido! <br/><br/>Hasta que lleguen nuevas instrucciones, reflexionad cómo habéis trabajado la misión:<br/><br/><b>¿Y si cambiaran los parámetros de esta?</b> </p>'
      }
    }
  }
</script>

