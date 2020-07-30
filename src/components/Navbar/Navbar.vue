<template>
  <div>
    <b-nav>
      <img :src="image" alt="" />
      <b-nav-item active><router-link to="/">Home</router-link></b-nav-item>
      <b-nav-item><router-link to="/about">About</router-link></b-nav-item>
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
      image: navImage,
    };
  },
};
</script>

<style></style>
