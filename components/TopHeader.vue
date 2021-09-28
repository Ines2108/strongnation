<template>
  <div class="top-header">
    <div class="spacer">
      <div class="logo">
        <nuxt-link to="/">
            <img src="../assets/homebutton.png" height="40" width="49">
        </nuxt-link>
      </div>
    </div>
    <div class="videos">
      <nuxt-link class="link" to="videos">
        Videos
      </nuxt-link>
    </div>
    <div class="aboutme">
      <nuxt-link class="link" to="aboutme">
        Über&nbsp;mich
      </nuxt-link>
    </div>
    <div class="contact">
      <nuxt-link class="link" to="contact">
        Kursinfo & Kontakt
      </nuxt-link>
    </div>
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
}
.link {
  color: black;
  text-decoration: none;
  font-family: arial;
}
.spacer {
  width: 79%;
}
.logo{
  padding: 15px;
}
.videos {
  padding: 25px;
}
.plan {
  padding: 25px;
}
.aboutme{
  padding: 25px;
}
.contact{
  padding: 25px;
}
</style>
