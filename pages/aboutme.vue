<template>
  <div class="about-me-body">
    <div class="elementor-row">
      <div class="elementor-left">
        <div class="about-me-section">
          <h2>ÜBER MICH<hr></h2>
          <div class="hey-ich-bin">
          <br><h3>Hey, ich bin Ines,</h3>
          <br><p>lizenzierte Zumba®- und STRONG Nation™-Trainierin, Tennisspielerin, Pizzaliebhaberin und Frohnatur, die es liebt,
          Leute in ihrem Kurs an ihre Grenzen zu bringen.</p>
          </div>
        </div>
      </div>
      <div class="elementor-right">
      </div>
    </div>
    <div class="short-description-box">
      <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
        sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
        no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
        sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.
        Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'aboutme'
}
</script>

<style scoped>
.about-me-body{
  background: linear-gradient(to right, whitesmoke, slategray);
  max-width: 1264px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  flex-flow: column;
  height:64vw;
  font-family: Verdana, Arial, Helvetica, sans-serif;
}
.elementor-row{
  display: flex;
  justify-content: flex-start;
  flex-direction: row;
  width: 131vh;
  height: 40vh;
  background-color: lightpink;
  margin-top: 10vh;
}
.elementor-left{
  display: flex;
  justify-content: left;
  width: 30vw;
  height: 29vw;
  padding-left: 10vh;
}
.about-me-section{
  width: 21vw;
  height: 10vh;
}
.elementor-right{
  display: flex;
  justify-content: right;
  width: 30vw;
  height: 26.5vw;
  background-image: url("~/assets/portrait_ines.jpg");
  background-size: cover;
  margin: 1em 3em 0vw 8vw;
  border: 0.5em solid #3e2b14;
}
.short-description-box{
  width: 30vw;
  height: 20vw;
  margin: 7vw 20vw 4vw 3vw;
}
</style>
