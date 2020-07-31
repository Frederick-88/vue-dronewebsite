<template>
  <div>
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
            <img src="../../assets/mydrone1.png" alt="image" class="drone-animation-fx" />
          </div>
          <div class="col-6 pl-4">
            <h1 class="display-4 title-fx text-white">Best quality Drone for your daily life</h1>
            <h5 class="text-white mt-4">
              Effects present letters inquiry no an removed or friends. Desire behind
              latter me though in. Supposing
              shameless am engrossed itatibus additions.
            </h5>
            <button class="btn bg-white mt-4">
              See More
              <i class="fas fa-arrow-alt-circle-down ml-2"></i>
            </button>
            <button>Tes</button>
          </div>
        </div>
      </div>
      <svg class="bottom-fx" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#ffffff" fill-opacity="1" d="M0,96L720,320L1440,96L1440,320L720,320L0,320Z" />
      </svg>
    </div>
    <div class="mt-5">Tes</div>
  </div>
</template>

<script>
// @ is an alias to /src
import navImage from "../../assets/logo-white.png";
import backgroundImage from "../../assets/bg.jpg";

export default {
  name: "Home",
  components: {},
  data() {
    return {
      image: navImage,
      backgroundImage: backgroundImage
    };
  }
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
