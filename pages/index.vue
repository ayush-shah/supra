<template>
  <div class="index">
    <div class="banner box">
      <p class="headline">SUPRA</p>
      <p>| Corrugated Box Manufacturer |<br>| Exported Quality Boxes |</p>
      <p class="year">Founded in 2016</p>
    </div>
    <div class="product box" id="product">
      <div class="section-title"><p>Our Products</p></div>
      <ProductBox class="product-body" />
    </div>
  </div>
</template>

<script>
import ProductBox from "@/components/productbox";
export default {
  name: "Index",
  components: { ProductBox },
};
</script>

<style scoped>
.box {
  position: relative;
}
.banner {
  width: 100%;
  position: relative;
  background: url("/supra/box01.jpg") no-repeat center;
  padding: 0;
  height: 100vh;
  background-size: cover;
  background-attachment: fixed;
  text-align: center;
  justify-content: center;
  display: flex;
  align-content: center;
  flex-flow: column wrap;
}
.banner:before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  background: #0005;
  width: 100%;
  height: 100vh;
  z-index: 1;
}
#product {
  width: 100%;
  position: relative;
  /* background: url("/supra/box2.jpg") no-repeat center; */
  padding: 0;
  min-height: 100vh;
  height: auto;
  background-size: cover;
  background-attachment: fixed;
}
.section-title p {
  padding: 2.5%;
  font-weight: 900;
  margin: 0;
  backdrop-filter: blur(10px);
  background: #fffa;
  color: #000;
}
.banner p {
  color: white;
  z-index: 3;
  margin: 0%;
}
p.headline {
  font-size: 1.2em;
  font-weight: 600;
  letter-spacing: 0.75em;
  width: 0;
  overflow: hidden;
  transition: all 1s;
  margin: 1.5% auto;
  animation: typewriter 2s 1s 1 both ease-in-out;
}
p.year {
  font-size: 0.8em;
  position: absolute;
  bottom: 0;
  right: 4%;
  margin: 1.5% 0;
}

.section-title {
  display: block;
  text-align: center;
  color: #ffffff;
  position: relative;
  letter-spacing: 0.25em;
  font-weight: 500;
  font-size: 1.12em;
}
.product-body {
  position: relative;
}
@keyframes typewriter {
  from {
    width: 0;
  }
  to {
    width: 50%;
  }
}
/* Responsive */
@media screen and (max-width: 480px) {
  .banner {
    height: 92vh;
  }
  .banner:before {
    height: 92vh;
  }
  .box {
    padding-bottom: 10vh;
  }
}
</style>
