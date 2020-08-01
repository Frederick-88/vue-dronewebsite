<template>
  <div>
    <Navbar />
    <div style="border-top:2px solid #2c3e50;">
      <div class="text-center" style="margin:2rem 16rem">
        <h3 class="icon-fx font-weight-bold">Review Form</h3>
        <h5 class="mt-4 font-weight-bold">1. Pick Your Character</h5>
        <div class="row d-flex justify-content-center">
          <div
            v-for="(character, index) in characters"
            :key="index"
            class="col-3 azur-border mx-2"
            :class="{
              activeBorder: selectedCharacter === character.characterGender,
            }"
            @click="updateSelectedCharacter(character.characterGender)"
          >
            <img
              :src="character.characterImage"
              alt="char-image"
              class="w-100"
            />
          </div>
        </div>
        <div>
          <h5 class="mt-4 font-weight-bold">2. Fill This Form</h5>
          <p class="mt-3 mb-1">Title of Review</p>
          <input
            name="title"
            type="text"
            class="w-75 py-2 px-3"
            placeholder="Title of Review"
            v-model="dataInput.title"
          />
          <p class="mt-3 mb-1">Description of Review</p>
          <input
            name="description"
            type="text"
            class="w-75 py-2 px-3"
            placeholder="Share with us how you felt on AzurDrones' Products!"
            v-model="dataInput.description"
          />
        </div>
      </div>

      <div class="text-center" style="margin:2rem 16rem">
        <h3 class="icon-fx font-weight-bold">The Review Data belongs here</h3>
        <button class="btn button-fx text-white">Button</button>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from "../Navbar/Navbar";
import Footer from "../Home/Footer";

export default {
  name: "Reviews",
  components: {
    Navbar,
    Footer,
  },
  data() {
    return {
      selectedCharacter: "Man",
      characters: [
        {
          characterGender: "Man",
          characterImage:
            "http://geniusdevs.com/themeforest/prolab/probucket/assets/images/testimonialimage/1.jpg",
        },
        {
          characterGender: "Women",
          characterImage:
            "http://geniusdevs.com/themeforest/prolab/probucket/assets/images/testimonialimage/2.jpg",
        },
      ],
      dataInput: {
        title: "",
        description: "",
      },
    };
  },
  methods: {
    updateSelectedCharacter(data) {
      this.selectedCharacter = data;
    },
  },
};
</script>

<style>
.azur-border {
  border: 2px solid rgba(44, 62, 80, 0.5);
  cursor: pointer;
}
.activeBorder {
  border: 2px solid rgba(44, 62, 80, 1);
}
</style>
