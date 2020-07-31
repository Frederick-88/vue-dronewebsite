<template>
  <div style="margin: 6rem 3rem">
    <h2 class="font-weight-bold text-center mb-4">Our Awesome Products</h2>

    <carousel :items="4" :nav="false" :loop="true" style="cursor:pointer;">
      <div>
        <div class="card mx-4" style="border: 2px solid rgba(0, 0, 0, 0.125);">
          <img
            src="../../assets/mydrone2.png"
            class="card-img-top w-100"
            style="height:150px"
            alt="..."
          />
          <div class="card-body">
            <div class="d-flex justify-content-center">
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star" style="color:#56eb00;"></i>
            </div>
            <div class="d-flex d-row mt-4 justify-content-center">
              <h4 class="icon-fx font-weight-bold">
                $136
              </h4>
              <h5 class="text-secondary ml-3"><del>$180</del></h5>
            </div>
            <h5 class="font-weight-bold text-center">Global Hawk</h5>
          </div>
        </div>
      </div>

      <div>
        <div class="card mx-4" style="border: 2px solid rgba(0, 0, 0, 0.125);">
          <img
            src="../../assets/mydrone3.png"
            class="card-img-top w-100"
            style="height:150px"
            alt="..."
          />
          <div class="card-body">
            <div class="d-flex justify-content-center">
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star text-secondary"></i>
            </div>
            <div class="d-flex d-row mt-4 justify-content-center">
              <h4 class="icon-fx font-weight-bold">
                $112
              </h4>
              <h5 class="text-secondary ml-3"><del>$150</del></h5>
            </div>
            <h5 class="font-weight-bold text-center">Pioneer</h5>
          </div>
        </div>
      </div>
      <div>
        <div class="card mx-4" style="border: 2px solid rgba(0, 0, 0, 0.125);">
          <img
            src="../../assets/mydrone4.png"
            class="card-img-top w-100"
            style="height:150px"
            alt="..."
          />
          <div class="card-body">
            <div class="d-flex justify-content-center">
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star" style="color:#56eb00;"></i>
            </div>
            <div class="d-flex d-row mt-4 justify-content-center">
              <h4 class="icon-fx font-weight-bold">
                $136
              </h4>
              <h5 class="text-secondary ml-3"><del>$180</del></h5>
            </div>
            <h5 class="font-weight-bold text-center">Shadow Air Force</h5>
          </div>
        </div>
      </div>
      <div>
        <div class="card mx-4" style="border: 2px solid rgba(0, 0, 0, 0.125);">
          <img
            src="../../assets/mydrone5.png"
            class="card-img-top w-100"
            style="height:150px"
            alt="..."
          />
          <div class="card-body">
            <div class="d-flex justify-content-center">
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star" style="color:#56eb00;"></i>
            </div>
            <div class="d-flex d-row mt-4 justify-content-center">
              <h4 class="icon-fx font-weight-bold">
                $198
              </h4>
              <h5 class="text-secondary ml-3"><del>$235</del></h5>
            </div>
            <h5 class="font-weight-bold text-center">Fire Scout</h5>
          </div>
        </div>
      </div>
      <div>
        <div class="card mx-4" style="border: 2px solid rgba(0, 0, 0, 0.125);">
          <img
            src="../../assets/mydrone1.png"
            class="card-img-top w-100"
            style="height:150px"
            alt="..."
          />
          <div class="card-body">
            <div class="d-flex justify-content-center">
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star mr-1" style="color:#56eb00;"></i>
              <i class="fas fa-star" style="color:#56eb00;"></i>
            </div>
            <div class="d-flex d-row mt-4 justify-content-center">
              <h4 class="icon-fx font-weight-bold">
                $136
              </h4>
              <h5 class="text-secondary ml-3"><del>$180</del></h5>
            </div>
            <h5 class="font-weight-bold text-center">Grey Eagle</h5>
          </div>
        </div>
      </div>
    </carousel>
  </div>
</template>

<script>
import carousel from "vue-owl-carousel";

export default {
  name: "CarouselPage",
  components: {
    carousel,
  },
};
</script>

<style></style>
