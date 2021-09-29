<template>
  <div class="top-header">
    <div class="toggle-button" type="button" @click.native="linkVisible= true">
      <span class="bar"></span>
      <span class="bar"></span>
      <span class="bar"></span>
    </div>
    <nuxt-link class="logo" to="/">
      <img src="../assets/homebutton.png" height="40" width="49">
    </nuxt-link>
    <div v-if="linkVisible" class="navbar" type="button" @close="close">
      <nuxt-link class="link" to="videos">
      Videos
      </nuxt-link>
      <nuxt-link class="link" to="aboutme">
      Über&nbsp;mich
      </nuxt-link>
      <nuxt-link class="link" to="contact">
      Kursinfo & Kontakt
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    linkVisible: true
  }),
  methods: {
    close () {
      this.linkVisible = false
    }
  },
  name: 'TopHeader'
}
</script>

<style scoped>
.top-header{
  background: linear-gradient(to right, deeppink, orangered);
  display: flex;
  justify-content: flex-start;
  align-items: center;
  padding: 1em;
  border-bottom: 1px solid black;
}
.navbar {
  display: flex;
}
.link {
  color: black;
  text-decoration: none;
  margin-left: 1em;
  font-size: 1.1em;
}
.toggle-button {
  position: absolute;
  top: 0.75em;
  right: 1em;
  display: none;
  flex-direction: column;
  justify-content: space-between;
  width: 30px;
  height: 21px;
  cursor: pointer;
}
.toggle-button .bar {
  height: 3px;
  width: 100%;
  background-color: black;
  border-radius: 10px;
}

@media (max-width: 480px) {
  .toggle-button {
    display: flex;
  }
  .link {
    display: none;
    padding: 0.5em;
  }
  .navbar {
    flex-direction: column;
  }
}
</style>
