<template>
  <div class="footer">
    <div class="footer-icons">
          <a href="https://www.facebook.com/ines.niedermaier/" target="_blank"><img src="../assets/FacebookIcon.png" height="40em" width="49em"></a>
          <a href="https://www.instagram.com/niedi_i/" target="_blank"><img src="../assets/NicePng_instagram-circle-logo-png_475136.png" height="40" width="49"></a>
    </div>
    <div class="footer-middle-section">
      <img src="../assets/thebeat.png" width="150" height="162" style="border-radius: 40%">
    </div>
    <div class="footer-link-section">
      <ul>
        <div>
          <nuxt-link class="footer-link" to="/">
            Startseite
          </nuxt-link>
        </div>
        <div>
          <nuxt-link class="footer-link" to="videos">
            Videos
          </nuxt-link>
        </div>
        <div>
          <nuxt-link class="footer-link" to="aboutme">
            Über&nbsp;mich
          </nuxt-link>
        </div>
        <div>
          <nuxt-link class="footer-link" to="contact">
            Kursinfo & Kontakt
          </nuxt-link>
        </div>
        <div>
          <nuxt-link class="footer-link" to="impressum">
            Impressum
          </nuxt-link>
        </div>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
.footer{
  background: black;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
}
@media (min-width:1024px) {
  .footer {
    flex-direction: row;
    justify-content: center;
  }
}
.footer-icons{
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 2em;
}
a {
  margin-right: 1em;
}
@media (min-width:1024px) {
  .footer-icons {
    flex-direction: column;
  }
  a{
    margin-bottom: 1em;
  }
}
.footer-middle-section {
  align-self: center;
}
.footer-link-section {
  display: flex;
  align-items: center;
}
.footer-link {
  text-decoration: none;
  color: white;
  line-height: 2em;
}
</style>
