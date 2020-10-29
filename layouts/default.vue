<template>
  <div class="mainBody">
    <Navbar />
    <Nuxt />
  </div>
</template>
<script>
import Navbar from "@/components/navbar";
export default {
  components: { Navbar },
};
</script>
<style>
* {
  box-sizing: border-box;
}
html,
body {
  margin: 0;
  padding: 0;
  font-family: "Poppins", sans-serif;
  scroll-behavior: smooth;
}
a {
  text-decoration: none;
  color: #fffe;
}
</style>
