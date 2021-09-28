<template>
<div class="bottom-footer">
  <div class="footer-left-section">
    <ul>
      <li>
        <a href="https://www.facebook.com/ines.niedermaier/" target="_blank"><img src="../assets/FacebookIcon.png" height="40em" width="49em"></a>
      </li>
      <li>
        <a href="https://www.instagram.com/niedi_i/" target="_blank"><img src="../assets/NicePng_instagram-circle-logo-png_475136.png" height="40" width="49"></a>
      </li>
    </ul>
  </div>
  <div class="footer-middle-section">
  </div>
  <div class="footer-right-section">
    <ul style="margin-top: 1vw">
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
.bottom-footer{
  display: flex;
  justify-content: center;
  position: inherit;
  background-color: black;
  height: 12vw;
}
.footer-left-section{
  display: flex;
  width: 10vw;
  align-items: center;
}
li {
  list-style-type: none;
}
li img {
  margin-top: 1em;
}
.footer-middle-section {
  align-self: center;
  background-image: url("~/assets/thebeat.png");
  background-position: center;
  background-size: cover;
  border-radius: 30%;
  width: 9vw;
  height: 8vw;
}
.footer-right-section {
  display: flex;
  align-items: center;
}
.footer-link {
  text-decoration: none;
  color: white;
}
</style>
