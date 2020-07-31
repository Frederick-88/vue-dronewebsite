<template>
  <div class="about">
    <Navbar />
    <h1>This is an about page</h1>
    <button class="btn button-fx text-white">Button</button>
  </div>
</template>

<script>
import Navbar from "../Navbar/Navbar";

export default {
  name: "About",
  components: {
    Navbar
  }
};
</script>
