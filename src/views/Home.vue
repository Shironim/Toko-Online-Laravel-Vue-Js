<template>
  <div class="home">
    <Header />
    <!-- <HeroShayna /> -->
    <!-- <WomanBanner />
    <InstaShayna />
    <PartnerShayna /> -->
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
// import HeroShayna from '@/components/HeroShayna.vue'
// import WomanBanner from '@/components/WomanBanner.vue'
// import InstaShayna from '@/components/InstaShayna.vue'
// import PartnerShayna from '@/components/PartnerShayna.vue'
import Footer from '@/components/Footer.vue'
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld
    Header,
    Footer,
    // HeroShayna,
    // WomanBanner,
    // InstaShayna,
    // PartnerShayna
  }
}
</script>
