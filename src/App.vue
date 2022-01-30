<template>
    <header>
      <Header></Header>
    </header>
    <router-view />

    <footer> 
      <Footer></Footer>
    </footer>

</template>

<script>
import Header from '../src/components/Header.vue'
import Footer from '../src/components/Footer.vue'
const API_URL = '/api/v1';

export default {
  components: { Header, Footer },
  
  mounted() {
    this.$store.dispatch('loadShowcase')
    this.$store.dispatch('loadCart')
  }
}
</script>

<style lang="scss">
  // * {
  //   padding: 0;
  //   margin: 0;
  // }

  // header {
  //   height: 80px;
  //   padding: 10px 20px;
  //   background: #ccc;
  //   display: flex;
  //   justify-content: space-between;
  //   align-items: center;
  //   margin-bottom: 50px;

  //   nav {
  //     display: flex;
  //     justify-content: space-between;
  //     width: 50%;
  //     align-items: center;
  //   }
  // }

  @import "@/styles/styles.scss";

</style>
