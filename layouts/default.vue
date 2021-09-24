<template>
<div>
  <TopHeader></TopHeader>
  <div ></div>
  <Nuxt></Nuxt>
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
}

</style>
