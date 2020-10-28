<template>
  <q-toolbar class="shadow-2" style="background-color: #ededf0;padding: 20px 0px;padding-left: 30px;">
    <q-btn flat label="Shoptop" />
    <q-space />
    <q-tabs v-model="tab" shrink>
      <q-tab name="tab1" label="home" clickable v-ripple :to="{name:'home'}"/>
      <q-btn-dropdown stretch flat label="Shop">
      <q-list>
        <q-item>
          <q-item-section>
            <q-item-label>Single Product</q-item-label>
          </q-item-section>
        </q-item>
        <q-item>
          <q-item-section>
            <q-item-label>Single Product details</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
      </q-btn-dropdown>
        <q-btn-dropdown stretch flat label="Pages">
        <q-list>
          <q-item>
            <q-item-section>
              <q-item-label>Tracking</q-item-label>
            </q-item-section>
          </q-item>
          <q-item>
            <q-item-section>
              <q-item-label>Checkout</q-item-label>
            </q-item-section>
          </q-item>
          <q-item>
            <q-item-section>
              <q-item-label>Elements</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>
      <q-tab name="blog" label="blog"/>
      <q-tab name="aboutus" label="about us"/>
    </q-tabs>
  </q-toolbar>
</template>


<template>
  <div class="q-pa-md banner">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
    >
      <q-carousel-slide :name="1" img-src="/banner_img.png" class="banner">
        <div class="absolute-bottom custom-caption">
          <div>Winter Fasion </br>Fashion Collection 2019</div>
          <a href="" class="text-subtitle1">Shop For Women</a>
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="1" img-src="/banner_img.png" class="banner">
        <div class="absolute-bottom custom-caption">
          <div>Winter Fasion </br>Fashion Collection 2019</div>
          <div class="text-subtitle1">Shop For Man</div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="1" img-src="/banner_img.png" class="banner">
        <div class="absolute-bottom custom-caption">
          <div>Winter Fasion </br>Fashion Collection 2019</div>
          <div class="text-subtitle1">Shop For Kid</div>
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>
</template>
<template>
  <div class="q-pa-md row q-gutter-md">
    <q-card class="my-card">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="title text-subtitle2 absolute-center text-center">
          Title
        </div>
      </q-img>
    </q-card>

    <q-card class="my-card">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="title text-h5 absolute-center text-right">
          Title
        </div>
      </q-img>
    </q-card>

    <q-card class="my-card">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="title text-h5 absolute-center text-right">
          Title
        </div>
      </q-img>
    </q-card>
  </div>
</template>

<style lang="sass">
.title
  width: 180px;
  height: 60px;
  text-align: center;
  font-size: 15px;
  font-weight: 500;
.my-card
  width: 100%
  max-width: 32%
.banner
  background-repeat: no-repeat;
  background-size: cover;
  height: 100%;
.custom-caption
  padding: 30px
  color: #000;

.text-subtitle1  
  display: inline-block;
  padding: 19px 61px;
  background-color: #2f7dfc;
  text-decoration: None;
  font-size: 15px;
  font-weight: 700;
  -webkit-transition: 0.5s;
  transition: 0.5s;
  text-transform: capitalize;
  color: #fff;
</style>
<script>
export default {
  data () {
    return {
      slide: 1
    }
  }
}
</script>
