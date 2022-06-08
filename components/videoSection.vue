<template>
  <div>
    <div class="container">
      <h1>DownLoad Our <span>APP</span></h1>
      <video width="720px" height="500px" loop="true" autoplay="autoplay">
        <source src="img/about/1.mp4" type="video/mp4" />
      </video>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  align-content: center;
  justify-content: center;
}
h1 {
  font-size: 3rem;
  font-weight: bold;
  font-family: 'Lato', cursive;
  margin-top: 2rem;
}
source {
  border-radius: 20px;
}

span {
  font-size: 3rem;
  font-weight: bold;
  color: brown;
  text-decoration: dotted underline;
  cursor: pointer;
}
</style>
