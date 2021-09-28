<template>
<div class="nuxtContainer">
  <TopHeader></TopHeader>
  <Nuxt style="display: flex; flex-direction: column;"></Nuxt>
  <Footer></Footer>
 </div>
</template>

<script>
import TopHeader from '~/components/TopHeader'
import Footer from '~/components/Footer'

export default {
  components: {
    TopHeader,
    Footer
  },
  name: 'default'
}

</script>

<style>
body {
  margin: 0;
  font-family: sans-serif;
}
</style>
