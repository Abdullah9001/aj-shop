<template>
  <div class="head">
    <div class="header">
      <h2>Aj-Shop</h2>
      <ul>
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/shop">Shop</NuxtLink></li>
        <li><NuxtLink to="/blog">Blog</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/contact">Contact</NuxtLink></li>
        <li>
          <NuxtLink to="/contact"
            ><img class="himg" src="img/shopping-bag.png"
          /></NuxtLink>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.head {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #e0dfdf;
  padding: 0 2rem;
  position: sticky;
}

h2 {
  font-size: 1.7rem;
  font-weight: bold;
  font-family: 'Pacifico', cursive;
  margin: 5px;
}

ul {
  display: flex;
  list-style: none;
}

li {
  padding: 10px;
  font-family: 'Lato', sans-serif;
}
a {
  text-decoration: none;
  color: black;
}

.himg {
  width: 20px;
  height: 20px;
}
</style>
