<template>
  <q-layout view="hHh LpR lfr">
    <q-header elevated height-hint="98">
      <q-toolbar class="shadow-2" style="background-color: #ededf0;padding: 20px 0px;padding-left: 30px;color:#000">
        <q-btn flat label="Shoptop" />
        <q-space />
        <q-tabs v-model="tab" shrink>
          <q-tab name="tab1" label="home" clickable v-ripple :to="{name:'home'}"/>
          <q-btn-dropdown stretch flat label="Shop">
          <q-list>
            <q-item clickable v-ripple :to="{name:'category'}">
              <q-item-section>
                <q-item-label>Product Category</q-item-label>
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
    </q-header>
    <q-carousel
      animated
      v-model="slide"
      arrows
      no-scroll
      navigation
      infinite
      class="no-scroll"
      style="margin-top:6.5%">
      <q-carousel-slide :name="1" no-scroll class="no-scroll" img-src="/banner_img.png">
        <div class="absolute-bottom custom-caption">
          Winter Fasion </br>Fashion Collection 2020</br>
          <a href="" class="text-subtitle1">Shop For Women</a>
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="2" no-scroll class="no-scroll" img-src="/offer-bg.png">
        <div class="absolute-bottom custom-caption">
          Winter Fasion </br>Fashion Collection 2020</br>
          <a href="" class="text-subtitle1">Shop For Kid</a>
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="3" no-scroll class="no-scroll" img-src="/arrivel/arrivel_6.png">
        <div class="absolute-bottom custom-caption">
          Winter Fasion </br>Fashion Collection 2020</br>
          <a href="" class="text-subtitle1">Shop For Age</a>
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="4" no-scroll class="no-scroll" img-src="/blog/single_blog_3.png">
        <div class="absolute-bottom custom-caption">
          Winter Fasion </br>Fashion Collection 2020</br>
          <a href="" class="text-subtitle1">Shop For Man</a>
        </div>
      </q-carousel-slide>
    </q-carousel>
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
          style="">
          <div class="absolute-center shopfor text-center">
            <a href="" style="text-decoration:none;color:#000;">Shop For Women</a>
          </div>
        </q-img>
      </div>
      <div class="col-4">
        <q-img
          src="/feature_3.png"
          style="">
          <div class="absolute-center shopfor text-center">
            <a href="" style="text-decoration:none;color:#000;">Shop For Kid</a>
          </div>
        </q-img>
      </div>
    </div>
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
  </q-layout>

</template>
<script>
export default {
  data () {
    return {
      slide: 1
    }
  }
}
</script>


<style lang="sass">

.scroll
  overflow: hidden!important;
.q-carousel
  margin-bottom: 5%;
.q-panel > div 
  height: 500px;
carousel__slides-container
  height: 160%;


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

