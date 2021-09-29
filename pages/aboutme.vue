<template>
  <div class="about-me">
    <h2>ÜBER MICH</h2>
    <div class="hey-ich-bin">
      <h3>Hey, ich bin Ines,</h3>
      <p>lizenzierte Zumba®- und STRONG Nation™-Trainierin, Tennisspielerin, Pizzaliebhaberin und Frohnatur, die es liebt,
        Leute in ihrem Kurs an ihre Grenzen zu bringen.</p>
    </div>
    <img class="image" src="~/assets/portrait_ines.jpg">
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat,
      sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
      no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
      sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.
      Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>
  </div>
</template>

<script>
export default {
  name: 'aboutme'
}
</script>

<style scoped>
.about-me {
  padding: 1em;
}
p {
  text-align: justify;
}
h2{
  border-bottom: 5px solid;
}
.image{
  border: 0.5em solid #3e2b14;
}
</style>
