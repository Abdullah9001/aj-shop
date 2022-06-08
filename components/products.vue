<template>
  <div>
    <div class="input">
      <input type="text" placeholder="Search Your Products" />
      <button>Search</button>
    </div>
    <div class="conteiner">
      <div id="card">
        <div
          class="card-content"
          v-for="(product, index) in products"
          :key="index"
        >
          <img class="pimage" :src="product.image" />
          <p>{{ product.company }}</p>
          <h5>{{ product.name }}</h5>
          <img class="picon" :src="product.icon" />
          <div class="card-flex">
            <p>{{ product.price }}</p>
            <NuxtLink to="/cart"
              ><img class="pcart" :src="product.cart"
            /></NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      search: '',
    }
  },
  computed: {
    products() {
      return this.$store.state.allProducts
    },
  },
}
</script>

<style scoped>
.input {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 2rem;
}

input {
  padding: 0.7rem;
  width: 250px;
  font-size: 0.8rem;
}

button {
  background-color: #d77e2a;
  color: #ffffff;
  border: none;
  padding: 0.7rem;
  font-size: 1rem;
  width: 100px;
  cursor: pointer;
}
.conteiner {
  display: flex;
}

#card {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 2rem;
  padding: 2rem;
}

.card-content {
  padding: 10px;
  margin: 10px;
  border: 1px solid #e0dfdf;
  border-radius: 0 20px 20px 20px;
  box-shadow: 4px 6px 9px -4px rgba(0, 0, 0, 0.87);
  -webkit-box-shadow: 4px 6px 9px -4px rgba(0, 0, 0, 0.87);
  -moz-box-shadow: 4px 6px 9px -4px rgba(0, 0, 0, 0.87);
}

.pimage {
  width: 250px;
  height: 250px;
  border-radius: 0 20px 20px 20px;
  object-fit: cover;
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

h5 {
  font-family: 'Lato', sans-serif;
  font-size: 1.3rem;
  color: #242222;
}

p {
  font-family: 'Lato', sans-serif;
  color: #716a6a;
}
</style>
