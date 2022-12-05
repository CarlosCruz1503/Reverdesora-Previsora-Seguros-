<template>
  <div class="home">
    <Header />
    <Radar id="radar"/>
    <Claves id="claves"/>
    <Services id="services" />
    <Table id="table"/>
    <Allies id="allies"/>
    <Faq />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Claves from '@/components/Claves.vue'
import Services from '@/components/Services.vue'
import Table from '@/components/Table.vue'
import Allies from '@/components/Allies.vue'
import Faq from '@/components/Faq.vue'
import Footer from '@/components/Footer.vue'
import Radar from '@/components/Radar.vue'
export default {
  name: 'HomeView',
  components: {
    Header, Claves, Services, Table, Allies, Faq, Footer, Radar
  }
}
</script>
