<template>
  <div class="home">
    <Gancho />
    <Header />
    <Radar id="radar"/>
    <ODS id="ods"/>
    <Claves id="claves"/>
    <Porque id="Porque"/>
    <Services id="services" />
    <Table id="table"/>
    <Allies id="allies"/>
    <Faq />
    <Team />
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
import ODS from '@/components/Ods.vue'
import Porque from '@/components/Porque.vue'
import Team from '@/components/Team.vue'
import Gancho from '@/components/Gancho.vue'
export default {
  name: 'HomeView',
  components: {
    Header, Claves, Services, Table, Allies, Faq, Footer, Radar, ODS, Porque, Team, Gancho
  }
}
</script>
