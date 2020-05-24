<template>
  <div class="product">
    <Header />
    <Breadcrumb />
    
    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="row">
                        <div class="col-lg-6">
                            <div class="product-pic-zoom">
                                      <!-- :src untuk binding data gambar, sesuai gambar yang dipilih di Product Thumbs-->
                                <img class="product-big-img" :src='gambar_default' alt="" />
                            </div>
                            <div class="product-thumbs">
                                <carousel :nav='false' :autoplay='true' :dots='false' class="product-thumbs-track ps-sliderl">
                                  <!-- on click event -> @click panggil fungsi ChangeImage dan rubah gambar class product-big-img sesuai url yang dikirim / bisa juga menggunakan array untuk API -->
                                    <div v-bind:class="thumbs[0] == gambar_default ? 'active' : ''" class="pt" @click="ChangeImage('img/mickey1.jpg')">
                                        <img src="img/mickey1.jpg" alt="" />
                                    </div>
                                    <!-- v-bind:class mengecek apakah nilai thumbs[] sesuai dengan nilai gambar_default, jika iya, tampilkan pada class product-big-img -->
                                    <div v-bind:class="thumbs[1] == gambar_default ? 'active' : ''" class="pt" @click="ChangeImage('img/mickey2.jpg')">
                                        <img src="img/mickey2.jpg" alt="" />
                                    </div>

                                    <div v-bind:class="thumbs[2] == gambar_default ? 'active' : ''" class="pt" @click="ChangeImage('img/mickey3.jpg')">
                                        <img src="img/mickey3.jpg" alt="" />
                                    </div>

                                    <div v-bind:class="thumbs[3] == gambar_default ? 'active' : ''" class="pt" @click="ChangeImage('img/mickey4.jpg')">
                                        <img src="img/mickey4.jpg" alt="" />
                                    </div>
                                </carousel>
                            </div>
                        </div>
                        <div class="col-lg-6">
                            <div class="product-details text-justify">
                                <div class="pd-title">
                                    <span>oranges</span>
                                    <h3>Pure Pineapple</h3>
                                </div>
                                <div class="pd-desc">
                                    <p>
                                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, error officia. Rem aperiam laborum voluptatum vel, pariatur modi hic provident eum iure natus quos non a sequi, id accusantium! Autem.
                                    </p>
                                    <p>
                                        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quam possimus quisquam animi, commodi, nihil voluptate nostrum neque architecto illo officiis doloremque et corrupti cupiditate voluptatibus error illum. Commodi expedita animi nulla aspernatur.
                                        Id asperiores blanditiis, omnis repudiandae iste inventore cum, quam sint molestiae accusamus voluptates ex tempora illum sit perspiciatis. Nostrum dolor tenetur amet, illo natus magni veniam quia sit nihil dolores.
                                        Commodi ratione distinctio harum voluptatum velit facilis voluptas animi non laudantium, id dolorem atque perferendis enim ducimus? A exercitationem recusandae aliquam quod. Itaque inventore obcaecati, unde quam
                                        impedit praesentium veritatis quis beatae ea atque perferendis voluptates velit architecto?
                                    </p>
                                    <h4>$495.00</h4>
                                </div>
                                <div class="quantity">
                                    <router-link to="/cart" >
                                      <a href="#" class="primary-btn pd-cart">Add To Cart</a>
                                    </router-link>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- Product Shop Section End -->
    
    <RelatedProduct />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import Header from "@/components/Header.vue";
import Breadcrumb from "@/components/Breadcrumb.vue";
import RelatedProduct from "@/components/RelatedProduct.vue";
import Footer from "@/components/Footer.vue";

import carousel from "vue-owl-carousel";

export default {
  name: "Product",
  components: {
    // HelloWorld
    Header,
    Footer,
    carousel,
    RelatedProduct,
    Breadcrumb
  },
  data(){
    return{
      gambar_default : "img/mickey1.jpg",
      thumbs: [
        "img/mickey1.jpg",
        "img/mickey2.jpg",
        "img/mickey3.jpg",
        "img/mickey4.jpg"
      ]
    }
  },
  methods: {
    ChangeImage(urlImg){
      this.gambar_default = urlImg;
    }
  },
};
</script>
<style scoped>
  .pt{
    margin-right: 10px;
  }
  /* .product-item:last-child{
    margin-right: 0;
  } */
</style>
