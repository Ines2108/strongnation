<template>
  <div class="body">
    <div class="header">
      <h1>STRONG NATION® by Ines Niedermaier</h1>
    </div>
    <div class="flex-image">
    <img src="../assets/flyer.png" height="900" width="614"/>
    </div>
    <p class="text">
      Was ist Strong Nation?
      STRONG NATION® ist ein revolutionäres, hochintensives Workout, das Dich an Deine Grenzen bringt. Die Musik ist eigens für die Workouts komponiert. Jede Kniebeuge, jeder Ausfallschritt und jede Bewegung hat ihre Entsprechung in den mitreißenden Beats. Werde eins mit der Musik und verausgabe Dich dabei vollkommen.
    </p>
  </div>
</template>

<script>

</script>

<style>
.header {
  background-color: slategray;
  border: 25pt pink;
  padding: 1vw 1vh;
  text-align: center;
}
@media(max-width: 700px){
  .body{
    background: black;
  }
}
.body {
  background: linear-gradient(to right, whitesmoke, slategray);
  max-width: 1264px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  flex-flow: column;
  height:95vh;
}
.flyer{
  width: 30vw;
  height: 30vh;
}
.flex-image {
  display: flex;
  justify-content: center;
  align-items: center;
}
.text {
  color:black;
  font-family: Carlito,sans-serif;
}
</style>
