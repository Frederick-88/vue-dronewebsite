<template>
  <div>
    <b-nav class="mx-5">
      <img :src="image" alt="navimage" class="nav-image" />
      <div class="ml-auto align-self-center">
        <router-link class="navlinks mr-3" to="/">Home</router-link>
        <router-link class="navlinks mr-3" to="/about">Products</router-link>
        <router-link class="navlinks mr-3" to="/about">Reviews</router-link>
        <router-link class="navlinks" to="/about">About</router-link>
      </div>
    </b-nav>
  </div>
</template>

<script>
import navImage from "../../assets/logo.png";
export default {
  name: "Navbar",
  components: {},
  data() {
    return {
      image: navImage
    };
  }
};
</script>

<style scoped>
.nav-image {
  width: 20rem;
}
.navlinks {
  color: #2c3e50;
  font-weight: 700;
}
</style>
