<template>
  <section class="section">
      <Banner />
      <Tabs />
  </section>
</template>

<script>
import Banner from '~/components/Banner'
import Tabs from '~/components/Tabs'

export default {
  name: 'HomePage',

  components: {
    Banner,
    Tabs
  }
}
</script>
