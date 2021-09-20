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
    <div class="description-box">
      <div class="image-box">
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
  height: 80vh;
  position: relative;
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
  font-family: "Droid Sans Mono Slashed";
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
.description-box{
  display: flex;
  justify-content: center;

}
.image-box{
  height: 311px;
  background: url("~/assets/strongleft.png");
}
</style>
