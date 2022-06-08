<template>
  <div>
    <div class="sImage">
      <div class="text">
        <h1>Sign Up For Newsletter</h1>
        <p>
          Get E-Mail Updates About Our Latest Shop and
          <span>Special Offers</span>
        </p>
      </div>
      <div class="input">
        <input type="text" placeholder="Enter Your Email" />
        <button>Sign Up</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.sImage {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 3rem;
  background-image: url('/img/banner/download.png');
  background-size: cover;
  background-repeat: no-repeat;
  padding: 4rem;
  width: 100%;
}

h1 {
  font-family: 'Lato', sans-serif;
  color: #ffffff;
}

p {
  font-family: 'Lato', sans-serif;
  color: #ffffff;
  margin-top: 5px;
  font-size: 0.8rem;
  word-spacing: 5px;
}

span {
  color: #d77e2a;
}

.input {
  display: flex;
  justify-content: center;
  align-items: center;
}

input {
  border: none;
  padding: 0.7rem;
  width: 250px;
  font-size: 0.8rem;
}

button {
  background-color: #d77e2a;
  color: #ffffff;
  border: none;
  padding: 0.7rem;
  font-size: 0.8rem;
  width: 100px;
  cursor: pointer;
}
</style>
