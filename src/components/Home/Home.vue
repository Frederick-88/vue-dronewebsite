<template>
  <div>
    <!-- This is the Section 1, the full view height -->
    <div class="home" :style="{ backgroundImage: `url(${backgroundImage})` }">
      <b-nav class="mx-5">
        <img :src="image" alt="navimage" class="nav-image" />
        <div class="ml-auto align-self-center">
          <router-link class="navlinks mr-3" to="/">Home</router-link>
          <router-link class="navlinks mr-3" to="/about">Products</router-link>
          <router-link class="navlinks mr-3" to="/about">Reviews</router-link>
          <router-link class="navlinks" to="/about">About</router-link>
        </div>
      </b-nav>
      <div class="border-top mx-3">
        <div class="row" style="margin-top: 7rem;">
          <div class="col-6">
            <img
              src="../../assets/mydrone1.png"
              alt="image"
              class="drone-animation-fx"
            />
          </div>
          <div class="col-6 pl-4">
            <h1 class="display-4 title-fx text-white">
              Best quality Drone for your daily life
            </h1>
            <h5 class="text-white mt-4">
              As the market leader in easy-to-fly drones and aerial photography
              systems, Azur Drones' quadcopters like the Phantom are the
              standard in consumer drone technology.
            </h5>
            <a href="#section2" class="btn bg-white mt-4">
              See More
              <i class="fas fa-arrow-alt-circle-down ml-2"></i>
            </a>
          </div>
        </div>
      </div>
      <svg
        class="bottom-fx"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1440 320"
      >
        <path
          fill="#ffffff"
          fill-opacity="1"
          d="M0,96L720,320L1440,96L1440,320L720,320L0,320Z"
        />
      </svg>
    </div>

    <!-- Section 2 -->
    <div id="section2" class="mt-5 text-center">
      <h2 class="font-weight-bold">Why AzurDrones Is Best</h2>
      <div style="margin: 1.5rem 10rem;">
        <div class="row">
          <div class="col-4">
            <div class="card">
              <div class="card-body">
                <i class="fas fa-undo-alt fa-3x icon-fx"></i>
                <h5 class="mt-3 font-weight-bold">1 Year Warranty</h5>
                <p>
                  Viewing hastily or written dearest elderly up weather.
                  direction so sweetness, Donec dearest justo.
                </p>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card">
              <div class="card-body">
                <i class="fas fa-shipping-fast fa-3x icon-fx"></i>
                <h5 class="mt-3 font-weight-bold">Free Delivery</h5>
                <p>
                  Viewing hastily or written dearest elderly up weather.
                  direction so sweetness, Donec dearest justo.
                </p>
              </div>
            </div>
          </div>
          <div class="col-4">
            <div class="card">
              <div class="card-body">
                <i class="fas fa-headset fa-3x icon-fx"></i>
                <h5 class="mt-3 font-weight-bold">Dedicated Support</h5>
                <p>
                  Viewing hastily or written dearest elderly up weather.
                  direction so sweetness, Donec dearest justo.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Section 3 -->
    <CarouselPage />

    <!-- Section 4 -->
    <h1>Choose us</h1>
    <i class="flaticon-photography"></i>
  </div>
</template>

<script>
// @ is an alias to /src
import navImage from "../../assets/logo-white.png";
import backgroundImage from "../../assets/bg.jpg";
import CarouselPage from "./Carousel";

export default {
  name: "Home",
  components: {
    CarouselPage,
  },
  data() {
    return {
      image: navImage,
      backgroundImage: backgroundImage,
    };
  },
};
</script>

<style>
.bottom-fx {
  z-index: 1;
  position: absolute;
  left: 0;
  bottom: 35px;
  width: 100%;
}

/* alternate = turn around */
/* in order to use z-index, you need to set the position as well. */
.drone-animation-fx {
  width: 95%;
  position: relative;
  z-index: 2;
  -webkit-animation: upsidedown 3s infinite alternate;
  animation: upsidedown 3s infinite alternate;
}

@keyframes upsidedown {
  0% {
    transform: translateY(80px);
  }
  100% {
    transform: translateY(0px);
  }
}
@-webkit-keyframes upsidedown {
  0% {
    transform: translateY(80px);
  }
  100% {
    transform: translateY(0px);
  }
}

.home {
  height: 94.7vh;
  background-size: cover;
  background-position: center;
}
.icon-fx {
  background: linear-gradient(55deg, #0250c5 0%, #d43f8d 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.nav-image {
  width: 20rem;
}
.navlinks {
  color: white;
  font-weight: 700;
}
.title-fx {
  font-family: "Russo One", sans-serif;
}
</style>
