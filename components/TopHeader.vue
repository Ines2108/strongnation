<template>
  <div class="top-header">
    <div class="toggle-button" type="button" @click="isMenuExpanded = !isMenuExpanded">
      <span class="bar" />
      <span class="bar" />
      <span class="bar" />
    </div>
    <nuxt-link class="logo" to="/">
      <img src="../assets/homebutton.png" height="40" width="49">
    </nuxt-link>
    <div class="navbar" type="button">
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
    <transition name="slide-fade">
      <div v-if="isMenuExpanded" class="menu-container">
        <div class="mobile-menu">
          <nuxt-link class="mobile-link" to="videos">
            Videos
          </nuxt-link>
          <nuxt-link class="mobile-link" to="aboutme">
            Über&nbsp;mich
          </nuxt-link>
          <nuxt-link class="mobile-link" to="contact">
            Kursinfo & Kontakt
          </nuxt-link>
        </div>
        <div class="black" />
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'TopHeader',
  data: () => ({
    isMenuExpanded: false
  }),
  methods: {
    close () {
      this.isMenuExpanded = false
    }
  }
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
  height: 3rem;
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
  top: 2em;
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
.logo {
  align-self: flex-start;
}
.menu-container{
  position: absolute;
  top: 4rem;
  left: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100vh;
}
.black {
  background-color: rgba(0, 0, 0, 0.5);
  height: 100%;
  width: 100vw;
}
.mobile-menu {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100vw;
  background: linear-gradient(to right, deeppink, orangered);
}
.mobile-link {
  color: black;
  align-self: center;
  text-decoration: none;
  margin-left: 1em;
  font-size: 1.1em;
  padding: 1em;
}
.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to
  /* .slide-fade-leave-active below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
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
@media (min-width: 481px) {
  .mobile-link {
    display: none;
  }
}
</style>
