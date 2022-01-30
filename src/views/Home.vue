<template>
<main>
    <section class="jumbotron-main">
        <div class="model container">
            <h1 class="brand-name">
                <span class="brand-bold">THE BRAND</span><br>
                OF LUXERIOUS <span class="brand-color">FASHION</span>
            </h1>
        </div>
    </section>

    <section class="offers">
        <div class="container">
            <div>
                <ul class="offers-list">
                    <li class="offer">
                        <img class="offer-img" src="../assets/for-women.png" alt="Offers for women" />
                        <div>
                            <span class="offer-span-us">30% OFF<br></span>
                            <span class="offer-span-pink">FOR WOMEN</span>
                        </div>
                    </li>
                    <li class="offer">
                        <img src="../assets/for-men.png" alt="Offers for men" />
                        <div>
                            <span class="offer-span-us">HOT DEAL<br></span>
                            <span class="offer-span-pink">FOR MEN</span>
                        </div>
                    </li>
                    <li class="offer">
                        <img src="../assets/for-kids.png" alt="Offers for kids" />
                        <div>
                            <span class="offer-span-us">NEW ARRIVALS<br></span>
                            <span class="offer-span-pink"> FOR KIDS</span>
                        </div>
                    </li>
                    <li class="offer last">
                        <img src="../assets/accesories.png" alt="Other offers" />
                        <div>
                            <span class="offer-span-us">LUXIROUS & TRENDY<br></span>
                            <span class="offer-span-pink"> ACCESORIES</span>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </section>

    <section class="items">
        <div class="container">
            <h2 class="items-heading center">Fetured Items</h2>
            <p class="items-about center">Shop for items based on what we featured in this week</p>

            <ul class="items-list">
                <ProductCard v-for="product of showcase" :key="product.id" :data="product" :target="'showcase'" v-on:productAction="onBuy" :amount="6"></ProductCard>
            </ul>
        </div>
        <div class="center items-button">
            <router-link to="/catalog" class="items-button-text">Browse All Products</router-link>
        </div>
    </section>

        <section class="services">
            <div class="container">
                <ul class="services-list">
                    <li class="service">
                        <div class="center">
                            <img src="../assets/delivery.svg" alt="delivery">
                        </div>
                        <div class="service-group">
                            <h2 class="service-heading">Free Delivery</h2>
                            <p class="service-text">Worldwide delivery on all. Authorit tively morph
                                next-generation
                                innovtion with extensive models.</p>
                        </div>
                    </li>
                    <li class="service">
                        <div class="center">
                            <img src="../assets/sales.svg" alt="sales">
                        </div>
                        <div class="service-group">
                            <h2 class="service-heading">Sales & discounts</h2>
                            <p class="service-text">Worldwide delivery on all. Authorit tively morph next-generation
                                innovtion with extensive models.</p>
                        </div>
                    </li>
                    <li class="service">
                        <div class="center">
                            <img src="../assets/quality.svg" alt="quality">
                        </div>
                        <div class="service-group">
                            <h2 class="service-heading">Quality assurance</h2>
                            <p class="service-text service-text-last">Worldwide delivery on all. Authorit tively morph
                                next-generation
                                innovtion with extensive models.</p>
                        </div>
                    </li>
                </ul>
            </div>
        </section>
</main>
</template>

<script>
import ProductCard from '../components/ProductCard.vue'

export default {
  components: { ProductCard },
  name: 'Home',
  computed: {
    showcase() {
      return this.$store.getters.getProducts
    }
  },
  methods: {
    onBuy(product) {
      this.$store.dispatch('addToCart', product)
    }
  }
}
</script>


<style lang="scss">
  .home{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 20px;
  }
</style>