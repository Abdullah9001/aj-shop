<template>
  <div>
    <div class="conteinerr">
      <h1>Feature Products</h1>
      <p>Summer Collections New Modern Design</p>
      <div id="cardd">
        <div
          class="card-contentt"
          v-for="(product, index) in products"
          :key="index"
        >
          <img class="pimage" :src="product.image" />
          <p>{{ product.company }}</p>
          <h4>{{ product.name }}</h4>
          <img class="picon" :src="product.icon" />
          <div class="card-flex">
            <p>{{ product.price }}</p>
            <NuxtLink to="/cart"
              ><img class="pcart" :src="product.cart"
            /></NuxtLink>
          </div>
        </div>
      </div>
      <div class="service">
        <div class="s-content">
          <p>Repair Service</p>
          <h1>Up To <span>70% Off </span> -All t-Shirt & Accessories.</h1>
          <NuxtLink to="/shop">Explore More</NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    products() {
      return this.$store.state.fProducts
    },
  },
}
</script>

<style scoped>
.conteinerr {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  font-family: 'Roboto', sans-serif;
  margin-top: 3rem;
  padding: 5px;
  word-break: 20px;
  color: #242222;
  word-spacing: 10px;
}

h4 {
  font-family: 'Lato', sans-serif;
  margin-top: 5px;
  color: #242222;
}

p {
  font-family: 'Lato', sans-serif;
  margin-top: 5px;
  color: #716a6a;
}
#cardd {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 2rem;
  padding: 0 3rem;
}

.card-contentt {
  padding: 10px;
  margin-top: 20px;
  border: 1px solid #e0dfdf;
  border-radius: 0 20px 0 20px;
  box-shadow: 4px 6px 9px -4px rgba(0, 0, 0, 0.87);
  -webkit-box-shadow: 4px 6px 9px -4px rgba(0, 0, 0, 0.87);
  -moz-box-shadow: 4px 6px 9px -4px rgba(0, 0, 0, 0.87);
}

.pimage {
  width: 250px;
  height: 250px;
  border-radius: 20px;
}

.picon {
  width: 80px;
  height: 20px;
}

.pcart {
  width: 20px;
  height: 20px;
}
.card-flex {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.service {
  margin-top: 4rem;
  background-image: url('/img/banner/b2.jpg');
  background-color: #cccccc;
  width: 100%;
  height: 100%;
}

.s-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 40vh;
}
.service p {
  font-family: 'Lato', sans-serif;
  color: #ffffff;
}

.service h1 {
  font-family: 'Lato', sans-serif;
  color: #ffffff;
  font-size: 2rem;
  font-weight: bold;
  margin-top: 10px;
}

.service a {
  margin-top: 10px;
  padding: 7px;
  background-color: #ffffff;
  color: #000000;
  font-family: 'Lato', sans-serif;
  text-decoration: none;
  border-radius: 5px;
}

span {
  color: #bb0e0e;
}
</style>
