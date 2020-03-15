<template>
  <div>
    <Header />
    <nuxt />
    <Footer />
    <GoTop
      :size="40"
      :left="15"
      :bottom="15"
      bg-color="rgba(0, 0, 0, 0.3)"
      :radius="7"
    />
  </div>
</template>

<script>
import GoTop from '@/components/GoTop'
import Header from '@/components/Header'
import Footer from '@/components/Footer'
export default {
  components: {
    Header,
    Footer,
    GoTop
  }
}
</script>

<style></style>
