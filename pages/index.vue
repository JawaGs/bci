<template>
  <section class="section">
      <Banner />
      <Tabs />

      
 
  </section>
</template>

<script>
import Card from '~/components/Card'
import Banner from '~/components/Banner'
import Tabs from '~/components/Tabs'

export default {
  name: 'HomePage',

  components: {
    Card,
    Banner,
    Tabs
  }
}
</script>
