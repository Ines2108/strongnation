<template>
  <div class="videoModal" @click="close">
    <div class="video">
      <div class="top">
        <img src="~/assets/close-button-png-30242.png" width="30" height="30">
      </div>
      <iframe
        src="https://player.vimeo.com/video/464298473?h=22f46e67c6"
        width="640"
        height="360"
        frameborder="0"
        allow="autoplay; fullscreen; picture-in-picture"
        allowfullscreen></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'VideoModal',
  methods: {
    close () {
      this.$emit('close')
    }
  }
}
</script>

<style scoped>
.videoModal{
  position: absolute;
  left: 0;
  top: 0;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: rgba(0,0,0,0.6);
}
.video{
  display: flex;
  flex-flow: column;
}
.top{
  display: flex;
  align-self: end;
  padding-bottom: 0.5em;
  cursor: pointer;
}
</style>
