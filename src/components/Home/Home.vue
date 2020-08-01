<template>
  <div>
    <!-- This is the Section 1, the full view height -->
    <div class="home" :style="{ backgroundImage: `url(${backgroundImage})` }">
      <b-nav class="mx-5">
        <img :src="image" alt="navimage" class="nav-image" />
        <div class="ml-auto align-self-center">
          <router-link class="navlinks mr-3" to="/">Home</router-link>
          <a class="navlinks mr-3" href="#products-section3">Products</a>
          <a class="navlinks mr-3" href="#features-section4">Features</a>
          <router-link class="navlinks mr-3" to="/reviews">Reviews</router-link>
          <a class="navlinks mr-3" href="#footer-section6">About</a>
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
            <h5 class="text-white mt-4 pr-5">
              As the market leader in easy-to-fly drones and aerial photography
              systems, Azur Drones' quadcopters like the Phantom are the
              standard in consumer drone technology.
            </h5>
            <a
              href="#section2"
              class="btn azur-btn-primary mt-4"
              style="position:relative; z-index:10"
            >
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
    <CarouselPage id="products-section3" />

    <!-- Section 4 -->
    <FeaturesPage id="features-section4" />

    <!-- Section 5 -->
    <div
      class="subscribe-bg"
      :style="{ backgroundImage: `url(${backgroundImage})` }"
    >
      <div class="text-center">
        <h2 class="font-weight-bold mb-3 text-white">
          Subscribe To Get Updates
        </h2>
        <p class="text-white mb-5">
          Prepared is me marianne pleasure likewise debating. Wonder an unable
          except better stairs do ye admire. His secure called esteem praise.
        </p>
        <div class="input-group">
          <input
            type="text"
            class="form-control py-4"
            placeholder="Your email address..."
          />
          <div class="input-group-append">
            <button
              @click="displayToast"
              class="btn btn-secondary"
              type="button"
              id="button-addon2"
            >
              Subscribe
              <i class="fas fa-paper-plane"></i>
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- Footer -->
    <FooterSection id="footer-section6" />
  </div>
</template>

<script>
// @ is an alias to /src
import navImage from "../../assets/logo-white.png";
import backgroundImage from "../../assets/bg.jpg";
import CarouselPage from "./Carousel";
import FeaturesPage from "./Features";
import FooterSection from "./Footer";

export default {
  name: "Home",
  components: {
    CarouselPage,
    FeaturesPage,
    FooterSection,
  },
  data() {
    return {
      image: navImage,
      backgroundImage: backgroundImage,
    };
  },
  methods: {
    displayToast() {
      this.$toast.info("Coming Soon for Subscribe Feature! Stay Tune.", {
        timeout: 3000,
        // the icon is available for fontawesome too!
        icon: "fab fa-vuejs",
      });
    },
  },
  mounted() {
    window.console.log("this is a log from mounted(useEffect in React)");
  },
};
</script>

<style>
.azur-btn-primary {
  background-color: white;
}
.azur-btn-primary:hover {
  background-color: black;
  color: white;
}
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
  color: rgb(200, 200, 200);
  font-weight: 700;
}
.navlinks:hover {
  color: white;
  text-decoration: none;
}
.subscribe-bg {
  background-size: cover;
  background-position: center;
  height: 100%;
  margin: 4rem 0;
  padding: 2rem 20rem;
}
.title-fx {
  font-family: "Russo One", sans-serif;
}
</style>
