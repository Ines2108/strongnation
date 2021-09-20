<template>
  <div class="body">
    <div class="flex-header">
      <div class="box-strong">
        <div class="erste-ueberschrift">
          <h1>Get Strong</h1>
        <div class="zweiter-text">
            <p>by Ines Niedermaier</p>
            <button class="button-style" type="button" @click="videoModalVisible = true">
             Vorschau ansehen
            </button>
        </div>
        </div>
      </div>
    </div>
    <video-modal v-if="videoModalVisible" @close="close">
    </video-modal>
    <div class="ff-block-wrap">
      <div class="ffb-image-wrap">
        <h2 class="was-ist-strong">Was ist Strong Nation?</h2>
      </div>
      <div class="ffb-content-wrap">
        <p class="descrition">STRONG Nation™ kombiniert Eigengewichts-, Muskelaufbau-, Kardio- und Plyometrietraining. Bewegt wird sich zu Originalmusik, die speziell auf jeden einzelnen Move abgestimmt wurde. Jede Kniebeuge, jeder Ausfallschritt, jeder Burpee wird von der Musik befeuert. So schaffst du es bis zur letzten Wiederholung – und hängst noch fünf weitere dran.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    videoModalVisible: false
  }),
  methods: {
    close () {
      this.videoModalVisible = false
    }
  }
}
</script>

<style>
.body {
  background: linear-gradient(to right, whitesmoke, slategray);
  max-width: 1264px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  flex-flow: column;
  height:180vh;
  font-family: "Droid Sans Mono Slashed";
}
.flex-header {
  background: url("~/assets/ines-background.jpg") no-repeat center;
  background-size: cover;
  height: 104vh;
  position: relative;
}
.box-strong{
  display: flex;
  justify-content: center;
  margin: 3em;
}
.button-style{
  border: 0;
  line-height: 2.5;
  padding: 0 20px;
  font-size: 1rem;
  text-align: center;
  color: #fff;
  text-shadow: 1px 1px 1px #000;
  border-radius: 10px;
  background-color: #ff4550;
  background-image: linear-gradient(to top left,
  rgba(0, 0, 0, .2),
  rgba(0, 0, 0, .2) 30%,
  rgba(0, 0, 0, 0));
  box-shadow: inset 2px 2px 3px rgba(255, 255, 255, .6),
  inset -2px -2px 3px rgba(0, 0, 0, .6);
}
.button-style:hover {
  background-color: orangered;
}
.ff-block-wrap{
  max-width: 67.8rem;
  display: flex;
  flex-flow: wrap;
  position: relative;
  padding-left: 13em;
  padding-bottom: 32em;
}
.ffb-image-wrap{
  display: flex;
  height: 350px;
  width: 501px;
  background: url("~/assets/strongleft.png");
}
.was-ist-strong {
  display: flex;
  height: 6vh;
  align-self: center;
  color: white;
  padding-right: 50%;
  margin-left: 10%;
}
.ffb-content-wrap{
  flex: 0 0 31%;
  min-height: 313px;
  background: black;
}
.descrition{
  color: white;
  height: 6vh;
  padding: 0.2em;
}
</style>
