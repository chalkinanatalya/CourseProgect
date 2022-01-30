<template>
  <div class="home">
    <!-- <product-card v-for="product of cart" :key="product.id" :data="product" :target="'cart'" v-on:productAction="onDelete"></product-card> -->
    <main>
    <section class="jumbotron">
        <div class="container brand-reg">
            <div>
                <h1 class="brand-header-reg">
                    SHOPPING CART
                </h1>
            </div>
        </div>
    </section>
    <section class="container">
        <div class="cart">
            <div class="cart-items">
              <CardInCart v-for="product of cart" :key="product.id" :data="product" :target="'cart'" v-on:productAction="onDelete"></CardInCart>
            </div>
            <div class="cart-buttons">
                <button class="cart-buttons-btn" onclick="clearSession()">Clear shopping card</button>
                <button class="cart-buttons-btn" onclick="window.location.href='catalog.html'">Continue shopping</button>
            </div>
            <div class="cart-order">
                <div class="cart-order-distribution">
                    <form action="#" class="cart-order-form">
                        <h2 class="cart-order-title">SHIPPING ADDRESS</h2>
                        <label><input type="text" required name="country" placeholder="Bangladesh"
                                class="cart-order-row"></label>
                        <label><input type="text" required name="state" placeholder="State"
                                class="cart-order-row"></label>
                        <label><input type="text" required name="email" placeholder="Postcode / Zip"
                                class="cart-order-row"></label>
                    </form>
                    <div>
                        <button class="cart-order-btn">GET A QUOTE</button>
                    </div>
                </div>
                <div class="cart-total">
                    <div class="cart-total-all">
                        <div class="cart-total-moveone">
                            <span class="cart-total-sub">SUB TOTAL</span>
                            <span class="cart-total-sub-price">$900</span>
                        </div>
                        <div class="cart-total-movetwo">
                            <span class="cart-total-grand">GRAND TOTAL</span> <span
                                class="cart-total-grand-price">$900</span>
                        </div>
                    </div>
                    <hr class="cart-total-hr">
                    <div class="cart-total-center">
                        <button class="cart-total-btn">PROCEED TO CHECKOUT</button>
                    </div>
                </div>
            </div>
        </div>
    </section>
    </main>
  </div>
</template>

<script>
import CardInCart from '../components/CardInCart.vue'

export default {
  components: { CardInCart },
  name: 'Cart',
  computed: {
    cart() {
      return this.$store.getters.getCart
    }
  },
  methods: {
    onDelete(product) {
      this.$store.dispatch('removeFromCart', product)
    }
  }
}
</script>