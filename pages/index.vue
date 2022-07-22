<template>
<div>
  <Header />
  <Nav />
  <h1>Hello, world!</h1>

</div>

</template>

<script>
import Header from '@/components/header/Header.vue'
//import Footer from '@/components/footer/Footer.vue'
//import About from '@/components/about/About.vue'
//import Contact from '@/components/contact/Contact.vue'
import Nav from '@/components/nav/Nav.vue'
//import Pilates from '@/components/pilates/Pilates.vue'
//import Time_price from '@/components/time_price/Time_price.vue'
export default {
  name: 'IndexPage',
  components: {
    Header,
    //Footer,
    //About,
    //Contact,
    Nav,
    //Pilates,
    //Time_price,
  }
}
</script>

<style lang="scss" scoped>


</style>