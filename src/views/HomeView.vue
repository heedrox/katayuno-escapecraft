<template>
  <div class="home-view">
    <h1>Bienvenido al Katayuno Escapecraft Edition</h1>
    <p><strong>Cómo jugar: </strong></p>
    <p> - Para comenzar la experiencia, abre las siguientes páginas en diferentes pestañas:</p>
    <ul>
      <li><a href="briefings" target="_blank">Las misiones</a></li>
      <li><a href="countdown" target="_blank">El contador de 3 horas</a></li>
      <li><a href="keypad1" target="_blank">El teclado de la misión 1</a></li>
      <li><a href="keypad3" target="_blank">El teclado kataboom!</a></li>
    </ul>
    <p> - Abre el sobre indicado como <b>NÚMERO 1</b>.</p>
    <p> - Léelo cuidadosamente y asegúrate que sabes qué hacer. Respira profundamente.</p>
    <p> - Ve al contador y pulsa START. No lo detengas a no ser que sea una emergencia.</p>
    <p> - Sigue las instrucciones de la misión durante las siguientes 3 horas. ¡Buena suerte, agente!</p>
    <hr>
    <p class="subline">By <a href="https://twitter.com/gonzalo123" target="_blank">@gonzalo123</a> and <a href="https://twitter.com/itortv" target="_blank">@itortv</a>.
      Thanks to <a href="https://twitter.com/ojoven" target="_blank">@ojoven</a> and <a href="https://twitter.com/540info" target="_blank">@540info</a></p>
  </div>
</template>
<style>
  @import url(https://fonts.googleapis.com/css?family=VT323:400);

  .home-view {
    text-align: left;
    padding-left: 10vw;
    padding-top: 8vh;
    font-size: 1vw;
  }

  .home-view h1,.home-view p {
    color: #999;
  }
  .home-view a {
    color: #006600;
  }
  .home-view h1,.home-view p,.home-view a {
    font-family: 'VT323', serif;
  }

  .home-view hr {
    margin-top: 75px;
    border-color: #444;
    color: #444;
  }

  .home-view .subline {
    color: #444;
  }
  @media screen and (orientation:portrait) {
    .home-view h1 {
      font-size: 4vh;
    }
    .home-view a, .home-view p {
      font-size: 3vh;
    }
    .home-view .subline, .home-view .subline a {
      font-size: 2vh;
    }

  }
  @media screen and (orientation:landscape) {
    .home-view h1 {
      font-size: 4vw;
    }
    .home-view a, .home-view p {
      font-size: 2vw;
    }
    .home-view .subline, .home-view .subline a {
      font-size: 1.5vw;
    }

  }
</style>
