<template>
  <q-toolbar class="shadow-2" style="background-color: #ededf0;padding: 20px 0px;padding-left: 30px;color:#000">
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