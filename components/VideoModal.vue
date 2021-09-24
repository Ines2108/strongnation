<template>
  <div class="videoModal" @click="close">
    <div class="video">
      <div class="top">
        <img src="~/assets/close-button-png-30242.png" width="30" height="30">
      </div>
      <iframe
        src="https://player.vimeo.com/video/612669466?h=a32d80c200&amp;title=0&amp;byline=0&amp;portrait=0&amp;speed=0&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479"
        width="312"
        height="640"
        frameborder="0"
        allow="autoplay; fullscreen; picture-in-picture"
        allowfullscreen
        title="STRONG Nation&amp;trade; by Ines">
      </iframe>
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
