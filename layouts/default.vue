<template>
  <div>
    <Header/>
    <Navigator/>
    <nuxt/>
    <Footer/>
  </div>
</template>

<script>
import Header from "~/components/common/Header";
import Navigator from "~/components/common/Navigator";
import Footer from "~/components/common/Footer";
export default {
  name: "default",
  components: {Footer, Navigator, Header},
}
</script>

<style scoped>

</style>
