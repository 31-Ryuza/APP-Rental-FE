<template>
  <div class="card shadow card-product">
    <img :src=" 'assets/images/' + product.photo " class="card-img-top" alt="..." />
    <div class="card-body">
      <h5 class="card-title">{{ product.name }}</h5>
      <p
        class="card-text"
      >Price : Rp. {{ product.price }} / Day</p>
      <router-link class="btn btn-warning" :to="'/foods/'+product.id"><b-icon-wallet></b-icon-wallet> Booking</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardProduct",
  props: ["product"],
};
</script>

<style>
</style>