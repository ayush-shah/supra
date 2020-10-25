<template>
  <div>
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
  font-family: Open Sans, sans-serif;
}
</style>
