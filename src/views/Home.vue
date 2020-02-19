<template>
  <div class="home">
    <Header></Header>
    <HeroImage></HeroImage>
    <PHP></PHP>
    <Pricin></Pricin>
    <Feature></Feature>
    <Include></Include>
    <Laravel></Laravel>
    <Module></Module>
    <Linux></Linux>
    <Share></Share>
    <Chat></Chat>
    <Footer></Footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HeroImage from '@/components/HeroImage.vue'
import PHP from '@/components/PHP.vue'
 import Pricin from '@/components/Price.vue'
import Feature from '@/components/Feature.vue'
import Include from '@/components/Include.vue'
import Laravel from '@/components/Laravel.vue'
import Module from '@/components/Module.vue'
import Linux from '@/components/Linux.vue'
import Share from '@/components/Share.vue'
import Chat from '@/components/Chat.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'home',
  components: {
    Header,
    HeroImage,
    PHP,
    Pricin,
    Feature,
    Include,
    Laravel,
    Module,
    Linux,
    Share,
    Chat,
    Footer
  }
}
</script>
