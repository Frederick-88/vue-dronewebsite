<template>
  <div className="mx-5 my-5">
    <div className="row">
      <div className="col-md-2">
        <img :src="navImage" alt="..." className="w-100" />
      </div>
      <div className="col-md-3">
        <p className="footer-title">S2 BOUTIQUE</p>
        <small>
          Look inside trendy,elegant & fantastic fashion in Batam. Tell the
          world who you are with style without having to speak.
        </small>
        <div className="mt-4">
          <small className="pt-4">© 2020 S2-Boutique Batam</small>
        </div>
      </div>

      <div className="col-md-3">
        <p className="footer-title">REACH OUT</p>
        <button className="btn btn-outline-success mr-3">
          <i className="fab fa-whatsapp fa-lg" />
        </button>

        <button className="btn btn-outline-instagram mr-3">
          <i className="fab fa-instagram fa-lg" />
        </button>
        <button className="btn btn-outline-primary mr-3">
          <i className="fab fa-facebook-square fa-lg" />
        </button>

        <button className="btn btn-outline-danger">
          <i className="far fa-envelope fa-lg" />
        </button>
      </div>
      <div className="col-md-4">
        <p className="footer-title">SUBSCRIBE</p>
        <small>
          Don't miss out the Latest Sale, Discounts, and New Arrivals !!
        </small>
        <div className="input-group mt-3 mb-2">
          <input
            type="email"
            className="form-control"
            name="emailUser"
            placeholder="Your Gmail/Email"
          />
          <div className="input-group-append">
            <button
              className="btn btn-outline-success"
              type="button"
              id="button-addon2"
            >
              <i className="fas fa-chevron-circle-right"></i>
            </button>
          </div>
        </div>
        <small className="text-secondary">
          We will not share your gmail/whatsapp to anyone else.
        </small>
      </div>
    </div>
  </div>
</template>

<script>
import navImage from "../../assets/logo.png";
export default {
  name: "FeaturesPage",
  components: {},
  data() {
    return {
      navImage: navImage,
    };
  },
};
</script>

<style></style>
