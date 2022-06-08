<template>
  <div>
    <div class="container">
      <img src="img/about/a6.jpg" />
      <div>
        <h1>Who we are.?</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam
          euismod, nisi vel consectetur euismod, nisi nisl consectetur nisi,
          eget consectetur nisi nisl eget nisi. Lorem ipsum dolor sit amet,
          consectetur adipisicing elit. Nulla sunt delectus ipsam natus laborum
          quis voluptates expedita fugit perferendis veritatis?
        </p>
        <p class="text1">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptate,
          culpa. Accusantium voluptas perferendis vel totam?
        </p>
        <p class="text2">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fugiat atque
          numquam dolor corporis distinctio molestiae!
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.container {
  margin-top: 3rem;
  display: flex;
  justify-content: center;
  align-items: center;
}
img {
  width: 500px;
  height: 400px;
  object-fit: cover;
  margin-right: 2rem;
}
h1 {
  font-weight: bold;
  font-family: 'Lato', cursive;
}

p {
  font-size: 1rem;
  font-family: 'Lato', sans-serif;
  color: #484747;
}

.text1 {
  text-decoration: dotted underline;
}
</style>
