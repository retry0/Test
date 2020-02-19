<template>
  <div class="home">
    <Header></Header>
    <HeroImage></HeroImage>
    <PHP></PHP>
    <Pricin></Pricin>
    <PowerFull></PowerFull>
    <Package></Package>
    <SupportLaravel></SupportLaravel>
    <Module></Module>
    <LinuxHosting></LinuxHosting>
    <Share></Share>
    <LiveChat></LiveChat>
    <Footer></Footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HeroImage from '@/components/HeroImage.vue'
import PHP from '@/components/PHP.vue'
 import Pricin from '@/components/Price.vue'
import PowerFull from '@/components/PowerfullPHP.vue'
import Package from '@/components/Package.vue'
import SupportLaravel from '@/components/LaravelSupport.vue'
import Module from '@/components/PHPModule.vue'
import LinuxHosting from '@/components/LinuxHosting.vue'
import Share from '@/components/Share.vue'
import LiveChat from '@/components/LiveChat.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'home',
  components: {
    Header,
    HeroImage,
    PHP,
    Pricin,
    PowerFull,
    Package,
    SupportLaravel,
    Module,
    LinuxHosting,
    Share,
    LiveChat,
    Footer
  }
}
</script>
