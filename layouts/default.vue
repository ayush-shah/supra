<template>
  <div class="mainBody">
    <Navbar />
    <Nuxt />
    <Sitemap />
  </div>
</template>
<script>
import Navbar from "@/components/navbar";
import Sitemap from "@/components/sitemap";
export default {
  components: { Navbar, Sitemap },
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
::-webkit-scrollbar {
  display: none;
}
</style>
