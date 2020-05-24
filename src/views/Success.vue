<template>
  <div class="success">
    <Header />
    <section>
      <div class="d-flex success-checkout align-items-center justify-content-center">
        <div class="col col-lg-4 text-center">
          <img src="img/success-buy.png" alt width="294" />
          <h3 class="mt-4">Sukses Terbayar!</h3>
          <p
            class="mt-2"
          >Silakan tunggu update terbaru dari kami via email yang sudah Anda daftarkan sebelumnya.</p>
          <router-link to="/" ><a href="#" class="primary-btn pd-cart mt-3">Back to Home</a></router-link>
        </div>
      </div>
    </section>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: "Home",
  components: {
    // HelloWorld
    Header,
    Footer
  }
};
</script>
