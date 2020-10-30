<!-- <template>
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
  <div class="row">
    <div class="col-4" >
      <q-img
        src="/feature_1.png">
        <div class="absolute-center shopfor text-center">
          <a href="" style="text-decoration:none;color:#000;">Shop For Man</a>
        </div>
      </q-img>
    </div>
    <div class="col-4">
      <q-img
        src="/feature_2.png"
        style="margin-left:10px;">
        <div class="absolute-center shopfor text-center">
          <a href="" style="text-decoration:none;color:#000;">Shop For Women</a>
        </div>
      </q-img>
    </div>
    <div class="col-4">
      <q-img
        src="/feature_3.png"
        style="margin-left:20px;">
        <div class="absolute-center shopfor text-center">
          <a href="" style="text-decoration:none;color:#000;">Shop For Kid</a>
        </div>
      </q-img>
    </div>
  </div>
</template>

<template>
  <div class="row" style="margin:5%;">
    <div class="col-3" >
      <div class="q-gutter-md" style="font-size: 2em">
        <q-icon name="today" style="color:#5595ff"/>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">Divided face for bearing the divide unto seed winged divided light Forth.</div>
      </div>
    </div>
    <div class="col-3" >
      <div class="q-gutter-md" style="font-size: 2em">
        <q-icon name="font_download" style="color:#5595ff"/>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">Divided face for bearing the divide unto seed winged divided light Forth.</div>
      </div>
    </div>
    <div class="col-3" >
      <div class="q-gutter-md" style="font-size: 2em">
        <q-icon name="warning" style="color:#5595ff"/>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">Divided face for bearing the divide unto seed winged divided light Forth.</div>
      </div>
    </div>
    <div class="col-3" >
      <div class="q-gutter-md" style="font-size: 2em">
        <q-icon name="format_size" style="color:#5595ff"/>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">Divided face for bearing the divide unto seed winged divided light Forth.</div>
      </div>
    </div>
  </div>
</template> -->
<template>
  <q-layout view="hHh LpR lfr">

    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="left = !left" />

        <q-toolbar-title>
          <q-avatar>
          </q-avatar>
          Title
        </q-toolbar-title>
      </q-toolbar>

      <q-tabs align="right">
        <q-route-tab to="/page1" label="Page One" />
        <q-route-tab to="/page2" label="Page Two" />
        <q-route-tab to="/page3" label="Page Three" />
      </q-tabs>
    </q-header>

    <q-drawer v-model="left" side="left" overlay>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quidem, eius reprehenderit eos corrupti
            commodi magni quaerat ex numquam, dolorum officiis modi facere maiores architecto suscipit iste
            eveniet doloribus ullam aliquid.
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<style lang="sass">
.text-subtitle2
  font-weight: normal;
  color: #606060;
.shopfor
  display: inline-block;
  width: 180px;
  height: 60px;
  background-color: #fff !important;
  font-size: 15px;

.shopfor:hover
  display: inline-block;
  width: 180px;
  height: 60px;
  background-color: #73d4d9 !important;
  font-size: 15px;

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
