<script>
  import HeaderView from './components/HeaderView.vue';
  import BannerView from './components/BannerView.vue';
  import SobreView from './components/SobreView.vue'
  import MetricasView from './components/MetricasView.vue'

  export default {
      components: {
        HeaderView,
        BannerView,
        SobreView,
        MetricasView
      }
  }
</script>

<template>
  <HeaderView  />
  <BannerView />
  <SobreView />
  <MetricasView />
</template>
