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
        <div class="row" style="margin-top: 5rem;">
          <div class="col-6">
            <img src="../../assets/mydrone1.png" alt="image" />
          </div>
          <div class="col-6">
            <h1 class="display-4 font-weight-bold text-white">Best quality Drone for your daily life</h1>
          </div>
        </div>
      </div>
      <svg class="bottom-fx" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#ffffff" fill-opacity="1" d="M0,96L720,320L1440,96L1440,320L720,320L0,320Z" />
      </svg>
    </div>
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
  position: absolute;
  left: 0;
  bottom: 35px;
  width: 100%;
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
</style>
