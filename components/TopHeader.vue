<template>
  <div class="top-header">
    <nuxt-link class="logo" to="/">
      <img src="../assets/homebutton.png" height="40" width="49">
    </nuxt-link>
    <nuxt-link class="link" to="videos">
      Videos
    </nuxt-link>
    <nuxt-link class="link" to="kursplan">
      Kursinfo
    </nuxt-link>
    <nuxt-link class="link" to="aboutme">
      Über&nbsp;mich
    </nuxt-link>
    <nuxt-link class="link" to="contact">
      Kontakt
    </nuxt-link>
  </div>
</template>

<script>
export default {
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
.link {
  color: black;
  text-decoration: none;
  margin-left: 1em;
  font-size: 1.1em;
}
</style>
