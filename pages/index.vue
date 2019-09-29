<template>
<div>
  <theme-carousel></theme-carousel>
  <time-event></time-event>
  <khatibs></khatibs>
  <theme-contact></theme-contact>
  <theme-map></theme-map>
  <theme-footer></theme-footer>
</div>

</template>

<script>
import Carousel from '@/components/Carousel'
import Welcom from '@/components/Welcom'
import Event from '@/components/Event'
import About from '@/components/About'
import Community from '@/components/Community'
import Donate from '@/components/Donate'
import Contact from '@/components/Contact'
import Map from '@/components/Map'
import Footer from '@/components/Footer'
import TimeEvent from '@/components/TimeEvent'
import Khatibs from '@/components/Khatibs'
export default {
  components : {
    themeCarousel: Carousel,
    themeWelcom: Welcom,
    themeEvent: Event,
    themeAbout: About,
    themeCommunity: Community,
    themeDonate: Donate,
    themeContact: Contact,
    themeMap: Map,
    themeFooter: Footer,
      TimeEvent,
      Khatibs
  }
}

</script>

<style>

</style>
