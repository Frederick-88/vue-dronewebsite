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
      <div class="border-top">
        <h1>
          Hi this is home with vue bootstrap
        </h1>
        <button class="btn button-fx text-white">Button</button>
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
        ></path>
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
      backgroundImage: backgroundImage,
    };
  },
};
</script>

<style>
.bottom-fx {
  position: absolute;
  left: 0;
  bottom: 15px;
  width: 100%;
}
.home {
  height: 97.7vh;
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
.button-fx {
  border: 0;
  padding: 0.75rem 1.5rem;
  background-image: linear-gradient(55deg, #0250c5 0%, #d43f8d 100%);
  transition: 0.3s ease-in;
}
.button-fx:hover {
  background-image: linear-gradient(55deg, #d43f8d 0%, #0250c5);
}
</style>
