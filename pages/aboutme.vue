<template>
  <div class="about-me">
    <div class="background-color" />
    <div class="information-about-me">
      <h2 class="title-about-me">ÜBER MICH</h2>
      <h3>Hey, ich bin Ines,</h3>
      <p>
        lizenzierte Zumba®- und STRONG Nation™-Trainierin, Tennisspielerin, Pizzaliebhaberin und Frohnatur, die es liebt,
        Leute in ihrem Kurs an ihre Grenzen zu bringen.
      </p>
    </div>
    <img class="image" src="~/assets/portrait_ines.jpg">
    <div class="description-me">
      <p>
        Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
        sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
        no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
        sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.
        Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Aboutme'
}
</script>

<style>
.about-me {
  display: flex;
  flex-direction: column;
  padding: 1em;
}
.background-color {
  position: absolute;
  z-index: 1;
  background-color: pink;
  height: 215px;
  width: 93%;
}
.information-about-me {
  width: auto;
  z-index: 2;
}
.title-about-me {
  border-bottom: 5px solid;
}
.image{
  border: 0.5em solid #3e2b14;
  z-index: 2;
}
.description-me {
  width: auto;
}
/*tablet version*/
@media (min-width: 480px) {
  .information-about-me {
    width: 60vw;
    z-index: 2;
  }
  .background-color {
    width: 85%;
    height: 310px;
  }
  .image {
    width: 30vw;
    height: 40vw;
    z-index: 2;
  }
}
  /*desktop version*/
@media (min-width: 1024px) {
    .about-me {
      flex-flow: row wrap !important;
      height: 60vw;
      margin-left: 3em;
      margin-right: 3em;
    }
    .information-about-me {
      position: relative;
      z-index: 2;
      width: 30vw;
      height: 20vw;
      top: 3em;
    }
    .image {
      position: relative;
      z-index: 1;
      left: 17em;
      top: 3em;
      width: 25vw;
      height: 35vw;
    }
    .background-color {
      width: 85%;
      z-index: 0;
      height: 20vw;
      padding: 2em;
    }
    .description-me {
      position: absolute;
      z-index: 2;
      width: 40vw;
      top: 28em;
    }
  }
@media (min-width: 1330px) {
  .about-me {
    height: 50vw;
    }
  .description-me {
    top: 35em;
   }
}
</style>
