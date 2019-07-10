<template>
<div>
  <theme-navbar></theme-navbar>
  <theme-carousel></theme-carousel>
  <theme-welcom></theme-welcom>
  <theme-event></theme-event>
  <theme-about></theme-about>
  <theme-community></theme-community>
  <theme-donate></theme-donate>
  <theme-contact></theme-contact>
  <theme-map></theme-map>
  <theme-footer></theme-footer>
</div>

</template>

<script>
import Navbar from '@/components/Navbar'
import Carousel from '@/components/Carousel'
import Welcom from '@/components/Welcom'
import Event from '@/components/Event'
import About from '@/components/About'
import Community from '@/components/Community'
import Donate from '@/components/Donate'
import Contact from '@/components/Contact'
import Map from '@/components/Map'
import Footer from '@/components/Footer'
export default {
  components : {
    themeNavbar: Navbar,
    themeCarousel: Carousel,
    themeWelcom: Welcom,
    themeEvent: Event,
    themeAbout: About,
    themeCommunity: Community,
    themeDonate: Donate,
    themeContact: Contact,
    themeMap: Map,
    themeFooter: Footer
  }
}

</script>

<style>

</style>
