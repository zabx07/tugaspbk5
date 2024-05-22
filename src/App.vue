<template>
  <div class="q-pa-md">
    <!-- Main Layout -->
    <q-layout view="lHh lpr lFf" container style="height: 4000px" class="shadow-2 rounded-borders">
      <!-- Navbar -->
      <q-header elevated class="bg-cyan">
        <q-toolbar>
          <q-btn flat round dense icon="store" label="My Store" aria-label="Go to My Store" />
          <q-space />
          <q-btn flat round dense icon="shopping_cart" class="q-mr-xs" aria-label="View Cart" />
          <q-btn flat round dense icon="account_circle" aria-label="Account" />
        </q-toolbar>

        <q-toolbar inset>
          <q-breadcrumbs active-color="white" style="font-size: 16px">
            <q-breadcrumbs-el label="Home" icon="home" />
            <q-breadcrumbs-el label="Products" icon="shopping_basket" />
            <q-breadcrumbs-el label="Contact" icon="contact_mail" />
          </q-breadcrumbs>
        </q-toolbar>
      </q-header>

      <!-- Page Container -->
      <q-page-container>
        <q-page class="q-pa-md">
          <!-- Carousel -->
          <q-carousel
            v-model="slide"
            transition-prev="slide-right"
            transition-next="slide-left"
            animated
            control-color="primary"
            class="rounded-borders q-mb-md"
          >
            <q-carousel-slide name="promo1" class="column no-wrap flex-center">
              <q-img src="./assets/P1.png" style="width: 100%;" alt="Promo 1" />
            </q-carousel-slide>
            <q-carousel-slide name="promo2" class="column no-wrap flex-center">
              <q-img src="./assets/p2.png" style="width: 100%;" alt="Promo 2" />
            </q-carousel-slide>
            <q-carousel-slide name="promo3" class="column no-wrap flex-center">
              <q-img src="https://via.placeholder.com/800x300?text=Promo+3" style="width: 100%;" alt="Promo 3" />
            </q-carousel-slide>
          </q-carousel>

          <!-- Product Cards -->
          <div class="row q-col-gutter-md q-mt-md">
            <q-card class="col-xs-12 col-sm-6 col-md-4 col-lg-3">
              <q-img src="./assets/gg.avif" style="height: 200px;" alt="Product 1">
                <q-card-section>
                  <div class="text-h6">60+60</div>
                  <div class="text-subtitle1">RP.69,000.</div>
                  <q-btn color="primary" label="Buy Now" class="q-mt-sm" aria-label="Buy Product 1" />
                </q-card-section>
              </q-img>
            </q-card>

            <q-card class="col-xs-12 col-sm-6 col-md-4 col-lg-3">
              <q-img src="./assets/gg.avif" style="height: 200px;" alt="Product 2">
                <q-card-section>
                  <div class="text-h6">128+128</div>
                  <div class="text-subtitle1">RP.120,000.</div>
                  <q-btn color="primary" label="Buy Now" class="q-mt-sm" aria-label="Buy Product 2" />
                </q-card-section>
              </q-img>
            </q-card>

            <q-card class="col-xs-12 col-sm-6 col-md-4 col-lg-3">
              <q-img src="./assets/gg.avif" style="height: 200px;" alt="Product 3">
                <q-card-section>
                  <div class="text-h6">360+360</div>
                  <div class="text-subtitle1">RP.400,000.</div>
                  <q-btn color="primary" label="Buy Now" class="q-mt-sm" aria-label="Buy Product 3" />
                </q-card-section>
              </q-img>
            </q-card>

            <q-card class="col-xs-12 col-sm-6 col-md-4 col-lg-3">
              <q-img src="./assets/gg.avif" style="height: 200px;" alt="Product 4">
                <q-card-section>
                  <div class="text-h6">880+880</div>
                  <div class="text-subtitle1">RP.990,000.</div>
                  <q-btn color="primary" label="Buy Now" class="q-mt-sm" aria-label="Buy Product 4" />
                </q-card-section>
              </q-img>
            </q-card>
          </div>
        </q-page>
      </q-page-container>

      <!-- Footer -->
      <q-footer class="bg-grey-8 text-white">
        <q-page class="q-pa-md">
          <div class="row justify-between">
            <div>
              <div class="text-h6">My Store</div>
              <div class="text-subtitle2">Best products, Best prices</div>
            </div>
            <div class="text-right">
              <q-btn flat round dense icon="facebook" aria-label="Facebook" />
              <q-btn flat round dense icon="twitter" aria-label="Twitter" />
              <q-btn flat round dense icon="instagram" aria-label="Instagram" />
            </div>
          </div>
        </q-page>
      </q-footer>
    </q-layout>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 'promo1'
    }
  }
}
</script>

<style>
.q-pa-md {
  padding: 16px;
}
.rounded-borders {
  border-radius: 8px;
}
.q-mb-md {
  margin-bottom: 16px;
}
</style>
