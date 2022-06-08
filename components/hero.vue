<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide class="image" img-src="/img/hero5.jpg">
        <div class="heroo">
          <div class="nothint">
            <p>Trade-in-offer</p>
            <h1 class="title">Super Value Deals</h1>
            <h1 class="title2">On All Products</h1>
            <p>Save more with coupons and up to 70% off.</p>
            <p class="btn"><NuxtLink to="/shop">Shop Now</NuxtLink></p>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide class="image" img-src="/img/hero1.jpg">
        <div class="heroo">
          <div class="nothint">
            <p>Trade-in-offer</p>
            <h1 class="title">Buy One Product</h1>
            <h1 class="title2">Get One Product Free</h1>
            <p>This is the offer you have nver seen</p>
            <p class="btn"><NuxtLink to="/shop">Shop Now</NuxtLink></p>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide class="image" img-src="/img/hero2.jpg">
        <div class="heroo">
          <div class="nothint">
            <p>Trade-in-offer</p>
            <h1 class="title">Seasonal Sale</h1>
            <h1 class="title2">Winter Collection 50% Off</h1>
            <p>Buy quickly,, It's for very short time</p>
            <p class="btn"><NuxtLink to="/shop">Shop Now</NuxtLink></p>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide class="image" img-src="/img/hero3.jpg">
        <div class="heroo">
          <div class="nothint">
            <p>Trade-in-offer</p>
            <h1 class="title">Upcoming Season</h1>
            <h1 class="title2">
              The best classic design in on sale at aj-shop
            </h1>
            <p>Save more with coupons and up to 70% off.</p>
            <p class="btn"><NuxtLink to="/shop">Shop Now</NuxtLink></p>
          </div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide class="image" img-src="/img/hero4.png">
        <div class="heroo">
          <div class="nothint">
            <p>Trade-in-offer</p>
            <h1 class="title">Super Value Deals</h1>
            <h1 class="title2">On All Products</h1>
            <p>Save more with coupons and up to 70% off.</p>
            <p class="btn"><NuxtLink to="/shop">Shop Now</NuxtLink></p>
          </div>
        </div>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      sliding: null,
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    },
  },
}
</script>

<style scoped>
.hero {
  background-image: url('/img/hero5.jpg');
  height: 92vh;
  background-size: cover;
  background-color: #cccccc;
  background-repeat: no-repeat;
}

.nothint {
  height: 80vh;
  width: 40%;
  padding-left: 4rem;
  font-family: 'Lato', sans-serif;
  line-height: 2.5rem;
  word-spacing: 5px;
}
.title2 {
  color: #0a6363;
  font-family: 'Roboto', sans-serif;
}
.btn {
  background-image: url('/img/button.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  padding-left: 30px;
  width: 10rem;
}
a {
  text-decoration: none;
  color: #0a6363;
  padding: 10px;
}

.image {
  width: 100%;
  height: 92vh;
}
</style>
