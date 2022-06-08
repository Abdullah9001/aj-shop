<template>
  <div>
    <mailSection />
    <div class="footer">
      <div class="contact">
        <h1>Aj Shop</h1>
        <h4>Contact</h4>
        <p class="mrt">
          <b>Address:</b> 38 bd road, Sirajganj Sadar, Sirajganj
        </p>
        <p><b>Phone:</b> +88 01717-XXXXXX</p>
        <p><b>Hours:</b>10:00 . 08:00 . Sut - Thus</p>
        <h4>Follow Us</h4>
        <div class="fimage">
          <img src="img/follow/facebook.png" />
          <img src="img/follow/instagram.png" />
          <img src="img/follow/twitter.png" />
          <img src="img/follow/youtube.png" />
        </div>
      </div>
      <div class="about">
        <h4>About</h4>
        <p class="mrt">About Us</p>
        <p>Delevary Information</p>
        <p>Privacy Policy</p>
        <p>Terms & Conditions</p>
        <p>Contact Us</p>
      </div>
      <div class="account">
        <h4>My Account</h4>
        <p class="mrt">Sign in</p>
        <p>Account</p>
        <p>My Account</p>
        <p>Order History</p>
        <p>Wish List</p>
        <p>Help</p>
      </div>
      <div class="install">
        <h4>Install App</h4>
        <p>From App Store or Google Play</p>
        <div class="pay-img">
          <img src="/img/pay/app.jpg" />
          <img src="/img/pay/play.jpg" />
        </div>
        <p>Secured Payment Galeways</p>
        <img src="img/pay/pay.png" />
      </div>
    </div>

    <div class="foot-txt">
      <p class="copy">
        <span> &copy; 2022 Aj Shop</span>
        <span>All Rights Reserved</span>
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.footer {
  display: flex;
  justify-content: center;
  align-items: center;
  justify-content: space-between;
  padding: 4rem;
}

.contact {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

h1 {
  font-size: 1.5rem;
  font-weight: bold;
  font-family: 'Pacifico', cursive;
}
.fimage {
  margin-top: 5px;
}

.fimage img {
  width: 20px;
  height: 20px;
  margin: 0 5px;
}

h4 {
  font-size: 1rem;
  font-weight: bold;
  font-family: 'Lato', sans-serif;
  margin-top: 10px;
}

p {
  font-size: 0.8rem;
  font-family: 'Lato', sans-serif;
  color: #716a6a;
}
b {
  color: #000000;
}

.mrt {
  margin-top: 10px;
}

.about p {
  margin-top: 5px;
}
.account p {
  margin-top: 5px;
}
.install p {
  margin-top: 5px;
}
.pay-img {
  margin-top: 5px;
}

.pay-img img {
  border: 1px solid #e0dfdf;
  border-radius: 5px;
}

.foot-txt {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 30px;
}
</style>
