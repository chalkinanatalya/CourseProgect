<template>
  <li v-if="data.id <= amount" class="item">
    <div class="item-overlay">
      <button v-on:click="onClick" class="item-btn" id="item5">Add to Cart</button>
    </div>
    <div class="item-img">
      <img :src="`${require('../assets/'+ data.img)}`" :alt="`${ data.title }`" width="360" height="420" />
    </div>
    <div class="item-group">
      <a href="#" class="item-title">{{ data.title.toUpperCase() }}</a>
      <p class="item-text">{{ data.description }}</p>
      <p class="item-price">{{ data.price }}$</p>
    </div>
  </li>

  <!-- <div class="card">
    <img :src="`./assets/${data.img}`" />
    <h3>{{ data.title }}</h3>
    <strong>{{ data.price }}$</strong>
    <button v-on:click="onClick" v-if="target == 'showcase'">Купить</button>
    <button v-on:click="onClick" v-if="target == 'cart'">Удалить</button>
  </div> -->
</template>

<script>
export default {
  name: "card",
  props: [
    "data",
    "target",
    "amount"
  ],
  methods: {
    onClick() {
      this.$emit('productAction', this.data)
    }
  }
}
</script>

<style lang="scss">
.card{
  width: 30%;
  border: 1px solid black;
  padding: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;

  img{
    width: 100%;
  }
}
</style>