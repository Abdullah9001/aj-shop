<template>
  <div>
    <div class="container" v-for="(blog, index) in blogs" :key="index">
      <img class="pimage" :src="blog.image" />
      <div class="text">
        <h3>{{ blog.title }}</h3>
        <p>{{ blog.description }}</p>
        <p class="bln">Continue Reading-------</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    blogs() {
      return this.$store.state.blogs
    },
  },
}
</script>

<style scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
}

.pimage {
  width: 350px;
  height: 220px;
  object-fit: cover;
  padding: 0.5rem;
  margin: 0.5rem;
}
h3 {
  font-family: 'Lato', sans-serif;
  margin-top: 5px;
  color: #242222;
}
p {
  font-family: 'Lato', sans-serif;
  margin-top: 5px;
  color: #716a6a;
}
.bln {
  cursor: pointer;
}
</style>
