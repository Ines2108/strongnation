<template>
  <div>
    <div class="flex-header">
      <div class="box-strong">
        <div class="title">Get Strong</div>
        <div class="subtitle">
          by Ines Niedermaier
        </div>
        <button class="button-style" type="button" @click="videoModalVisible = true">
          Vorschau ansehen
        </button>
      </div>
    </div>
    <video-modal v-if="videoModalVisible" @close="close"></video-modal>
    <div class="ff-block-wrap">
      <div class="ffb-image-wrap">
        <h2 class="was-ist-strong">Was ist STRONG Nation™?</h2>
      </div>
      <div class="ffb-content-wrap">
        <diy class="description">
          <p>STRONG Nation™ kombiniert Eigengewichts-, Muskelaufbau-, Kardio- und Plyometrietraining.
            Bewegt wird sich zu Originalmusik, die speziell auf jeden einzelnen Move abgestimmt wurde. Jede Kniebeuge, jeder Ausfallschritt,
            jeder Burpee wird von der Musik befeuert. So schaffst du es bis zur letzten Wiederholung – und hängst noch fünf weitere dran.</p>
        </diy>
        <div class="link-style">
          <a class="link-text" href="https://strong.zumba.com/de-DE/pages/class" target="_blank">Erfahre Mehr</a>
        </div>
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
.flex-header {
  background: url("~/assets/ines-background.jpg") no-repeat center;
  background-size: cover;
  direction: rtl;
  min-height: max(30em, 40vw);
}
.box-strong{
  display: flex;
  flex-flow: column;
  width: 20vw;
  margin: 2em;
  margin-right: 15vw;
}
.title {
  font-size: 2.5em;
  white-space: nowrap;
}
.subtitle {
  font-size: 1.2em;
  white-space: nowrap;
}
.button-style{
  margin-top: 1em;
  border: 0;
  line-height: 2.5;
  padding: 0 20px;
  width: 15em;
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
  display: flex;
  flex-flow: wrap;
  width: 100%;
}
.ffb-image-wrap{
  display: flex;
  width: 100%;
  height: 50vw;
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
  width: 100%;
  background: black;
  padding: 1%;
}
.description{
  width: 100%;
  color: white;
  height: 6vh;
  padding: 0.2em;
}
.link-style{
  display: flex;
  justify-content: center;
  background: 0 0;
  box-shadow: inset 0 0 0 2px #ff6248;
  padding: .75em 2em .7em;

}
.link-text{
  text-decoration: none;
  color: #ff6248;
  text-transform: uppercase;
}
</style>
