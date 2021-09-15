<template>
  <div class="top-header">
    <div class="spacer">
      <div class="logo">
        <nuxt-link to="/">
            <img src="../assets/homelogo.png" height="86" width="66">
        </nuxt-link>
      </div>
    </div>
    <div class="videos">
      <nuxt-link class="link" to="videos">
        Videos
      </nuxt-link>
    </div>
    <div class="plan">
      <nuxt-link class="link" to="kursplan">
        Kursplan
      </nuxt-link>
    </div>
    <div class="instructor">
      <nuxt-link class="link" to="instructor">
        Instructor
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
  width: 40%;
}
.videos {
  padding: 30px;
  font-family: Dialog, Serif !important;
}
.plan {
  padding: 30px;
}
.instructor {
  padding: 30px;
}
</style>
