<template>
  <q-layout view="hHh LpR lfr">

    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="left = !left" />

        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
          </q-avatar>
          Title
        </q-toolbar-title>
      </q-toolbar>

      <q-tabs align="left">
        <q-route-tab to="/page1" label="Page One" />
        <q-route-tab to="/page2" label="Page Two" />
        <q-route-tab to="/page3" label="Page Three" />
      </q-tabs>
    </q-header>

    <q-drawer v-model="left" side="left">
      <q-list style="margin:40% 0 0 20%;">
        <q-item>
          <q-item-section class="browse_category">BROWSE CATEGORIES</q-item-section>
        </q-item>
      <q-expansion-item
        expand-separator
        icon="perm_identity"
        label="Shoe"
      >
        <q-item>
          <q-item-section>Wellington Boots</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>high heel</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Gladiator sandals</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Court Shoes</q-item-section>
        </q-item>
      </q-expansion-item>
      <q-expansion-item
        expand-separator
        icon="perm_identity"
        label="Shoe"
      >
        <q-item>
          <q-item-section>Wellington Boots</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>high heel</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Gladiator sandals</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Court Shoes</q-item-section>
        </q-item>
      </q-expansion-item>
      <q-expansion-item
        expand-separator
        icon="perm_identity"
        label="Shoe"
      >
        <q-item>
          <q-item-section>Wellington Boots</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>high heel</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Gladiator sandals</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Court Shoes</q-item-section>
        </q-item>
      </q-expansion-item>
      <q-expansion-item
        expand-separator
        icon="perm_identity"
        label="Shoe"
      >
        <q-item>
          <q-item-section>Wellington Boots</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>high heel</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Gladiator sandals</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Court Shoes</q-item-section>
        </q-item>
      </q-expansion-item>
      <q-expansion-item
        expand-separator
        icon="perm_identity"
        label="Shoe"
      >
        <q-item>
          <q-item-section>Wellington Boots</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>high heel</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Gladiator sandals</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Court Shoes</q-item-section>
        </q-item>
      </q-expansion-item>
      <q-expansion-item
        expand-separator
        icon="perm_identity"
        label="Shoe"
      >
        <q-item>
          <q-item-section>Wellington Boots</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>high heel</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Gladiator sandals</q-item-section>
        </q-item>
        <q-item>
          <q-item-section>Court Shoes</q-item-section>
        </q-item>
      </q-expansion-item>
      <q-item>
        <q-item-section class="browse_category">BROWSE BRANDS</q-item-section>
      </q-item>
      <q-option-group
      :options="brands"
      label="Notifications"
      type="radio"
      v-model="group"
      />
      <q-item>
        <q-item-section class="browse_category">BROWSE COLORS</q-item-section>
      </q-item>
      <q-option-group
      :options="color"
      label="Notifications"
      type="radio"
      v-model="group"
      />
      <q-item>
        <q-item-section class="browse_category">PRICE FILTER</q-item-section>
      </q-item>
      <q-range
        v-model="label"
        :min="0"
        :max="50000"
        :step="5"
        label
        color="secondary"
      />
      <q-badge color="secondary" class="q-mb-lg">
        Model: {{ label.min }} to {{ label.max }} (0 to 50000, step 5)
      </q-badge>
    </q-list>
    </q-drawer>

    <q-page-container>
      <div class="row" style="margin-left:10%;">
        <div class="col-4" >
          <q-card class="my-card">
            <q-img
              src="/feature_1.png">
            </q-img>
            <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-4" >
          <q-card class="my-card">
            <q-img
              src="/feature_1.png">
            </q-img>
            <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-4" >
          <q-card class="my-card">
            <q-img
              src="/feature_1.png">
            </q-img>
            <q-card-section>
              <div class="text-h6">Our Changing Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </q-page-container>

  </q-layout>
</template>

<script>
export default {
  data () {
    return {
      left: true,
      group: null,
      brands: [
        { label: 'Nike', value: 'Nike' },
        { label: 'Addidas', value: 'Addidas'},
        { label: 'Reebok', value: 'Reebok'},
        { label: 'Puma', value: 'Puma'},
        { label: 'Brooks', value: 'Brooks'}
      ],
      color: [
        { label: 'Black', value: 'Black' },
        { label: 'Gold', value: 'Gold'},
        { label: 'White', value: 'White'},
        { label: 'Blue', value: 'Blue'},
        { label: 'Lite Dark', value: 'Lite'}
      ],
      label: {
        min: 0,
        max: 50000
      }
    }
  }
}
</script>

<style lang="sass">
.browse_category
  margin-bottom: 20px;
  font-size: 14px;
  font-family: "Roboto", sans-serif;
  color: #2a2a2a;
  font-weight: 500;
  line-height: 40px;
  position: relative;
  background-color: #e8f0f2;
  padding: 10px 15px 10px 30px;
.my-card
  width: 100%
  max-width: 250px
</style>