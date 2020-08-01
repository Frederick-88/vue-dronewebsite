<template>
  <div class="mx-1 footer-bg" :style="{ backgroundImage: `url(${footerImage})` }">
    <div class="text-center">
      <img :src="navImage" alt="..." style="width:20rem" />
    </div>
    <p
      class="text-center text-secondary"
      style="margin:0 12rem"
    >As the market leader in easy-to-fly drones and aerial photography systems, Azur Drones' quadcopters like the Phantom are the standard in consumer drone technology.</p>
    <div class="d-flex justify-content-center mt-4">
      <button class="btn btn-outline-success mr-3">
        <i class="fab fa-whatsapp fa-lg" />
      </button>

      <button class="btn btn-outline-instagram mr-3">
        <i class="fab fa-instagram fa-lg" />
      </button>
      <button class="btn btn-outline-primary mr-3">
        <i class="fab fa-facebook-square fa-lg" />
      </button>

      <button class="btn btn-outline-danger">
        <i class="far fa-envelope fa-lg" />
      </button>
    </div>
    <div class="mt-4 border-top">
      <p class="text-center pt-3 text-secondary">
        Copyright © 2020. All rights reserved by
        <span class="icon-fx">Chen Frederick</span>
      </p>
    </div>
  </div>
</template>

<script>
import navImage from "../../assets/logo.png";
import footerImage from "../../assets/footer-bg.png";
export default {
  name: "FeaturesPage",
  components: {},
  data() {
    return {
      navImage: navImage,
      footerImage: footerImage
    };
  }
};
</script>

<style>
.btn-outline-instagram {
  color: #fb3958 !important;
  border-color: #fb3958 !important;
}
.btn-outline-instagram:hover {
  color: #fff !important;
  background-color: #fb3958 !important;
  border-color: #fb3958 !important;
}
.btn-outline-instagram:focus {
  box-shadow: 0 0 0 0.2rem rgba(220, 53, 69, 0.5) !important;
}
.footer-bg {
  background-size: cover;
  background-position: center;
  height: 100%;
  padding: 2rem 0;
}
</style>
