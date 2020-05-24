<template>
  <!-- Header Section Begin -->
  <header class="header-section">
    <div class="header-top">
      <div class="container">
        <div class="ht-left">
          <div class="mail-service">
            <i class="fa fa-envelope"></i> hello.shayna@gmail.com
          </div>
          <div class="phone-service">
            <i class="fa fa-phone"></i> +628 22081996
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="inner-header">
        <div class="row">
          <div class="col-lg-2 col-md-2">
            <div class="logo">
              <router-link to="/">
                <img src="img/logo_website_shayna.png" alt />
              </router-link>
            </div>
          </div>
          <div class="col-lg-7 col-md-7"></div>
          <div class="col-lg-3 text-right col-md-3">
            <ul class="nav-right">
              <li class="cart-icon">
                Keranjang Belanja &nbsp;
                <a href="#">
                  <i class="icon_bag_alt"></i>
                  <span>3</span>
                </a>
                <div class="cart-hover">
                  <div class="select-items">
                    <table>
                      <tbody>
                        <tr>
                          <td class="si-pic">
                            <img src="img/select-product-1.jpg" alt />
                          </td>
                          <td class="si-text">
                            <div class="product-selected">
                              <p>$60.00 x 1</p>
                              <h6>Kabino Bedside Table</h6>
                            </div>
                          </td>
                          <td class="si-close">
                            <i class="ti-close"></i>
                          </td>
                        </tr>
                        <tr>
                          <td class="si-pic">
                            <img src="img/select-product-2.jpg" alt />
                          </td>
                          <td class="si-text">
                            <div class="product-selected">
                              <p>$60.00 x 1</p>
                              <h6>Kabino Bedside Table</h6>
                            </div>
                          </td>
                          <td class="si-close">
                            <i class="ti-close"></i>
                          </td>
                        </tr>
                      </tbody>
                    </table>
                  </div>
                  <div class="select-total">
                    <span>total:</span>
                    <h5>$120.00</h5>
                  </div>
                  <div class="select-button">
                    <a href="#" class="primary-btn view-card">VIEW CARD</a>
                    <a href="#" class="primary-btn checkout-btn">CHECK OUT</a>
                  </div>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </header>
  <!-- Header End -->
</template>
<script>
export default {
  name: 'Header',
  components: {
    // HelloWorld
  }
}
</script>