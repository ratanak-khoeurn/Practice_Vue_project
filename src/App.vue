<template>
  <div>
    <nevigation-bar-vue></nevigation-bar-vue>
    <header-vue></header-vue>
    <section class="container mt-4" style="margin-left: 95px;width: 84%;">
        <h3>All products</h3>
        <div class="row mt-3">
          <card-base-vue v-for="i in 10" :key="i"></card-base-vue>
        </div>
    </section>
  </div>
</template>

<script>
import NevigationBarVue from './components/NevigationBar.vue'
import HeaderVue from './components/HeaderVue.vue'
import CardBaseVue from './components/CardBase.vue'
export default {
  name: 'App',
  components: {
    NevigationBarVue,
    HeaderVue,
    CardBaseVue,
  },
  data() {
    return {
      message: 'Welcome to Your Vue.js App',
    }
  },
}
</script>
