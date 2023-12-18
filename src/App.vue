<script>
  import HeaderView from '@/components/HeaderView.vue'
  import BannerView from '@/components/BannerView.vue'
  import SobreView from '@/components/SobreView.vue'
  import RecursosView from '@/components/RecursosView.vue'
  import MetricasView from '@/components/MetricasView.vue'
  import ComidaView from '@/components/ComidaView.vue'
  import ParceirosView from '@/components/ParceirosView.vue'
  import NewletterView from '@/components/NewsletterView.vue'
  import Rodape from '@/components/RodapeView.vue'

  export default {
      components: {
        HeaderView,
        BannerView,
        SobreView,
        RecursosView,
        MetricasView,
        ComidaView,
        ParceirosView,
        NewletterView,
        Rodape
      }
  }
</script>

<template>
  <HeaderView  />
  <BannerView />
  <SobreView />
  <RecursosView />
  <MetricasView />
  <ComidaView />
  <ParceirosView />
  <NewletterView />
  <Rodape />
</template>
