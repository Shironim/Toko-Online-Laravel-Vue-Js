<template>
    <!-- Hero Section Begin -->
    <section class="hero-section">
      <carousel :nav='false' :autoplay='true' :items=1 class="hero-items">
        <div class="single-hero-items set-bg" style="background:url(img/hero-1.jpg)">
          <div class="container">
            <div class="row">
              <div class="col-lg-5">
                <span>Bag,kids</span>
                <h1>Black friday</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div>
        <div class="single-hero-items set-bg" style="background:url(img/hero-2.jpg)">
          <div class="container">
            <div class="row">
              <div class="col-lg-5">
                <span>Bag,kids</span>
                <h1>Black friday</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div>
        <div class="single-hero-items set-bg" style="background:url(img/hero-3.jpg)">
          <div class="container">
            <div class="row">
              <div class="col-lg-5">
                <span>Bag,kids</span>
                <h1>Black friday</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                <a href="#" class="primary-btn">Shop Now</a>
              </div>
            </div>
          </div>
        </div>

      </carousel>
    </section>
    <!-- Hero Section End -->
</template>
<script>
import carousel from "vue-owl-carousel";

export default {
  name:'HeroShayna',
  components : {
    carousel,
  }  
}
</script>