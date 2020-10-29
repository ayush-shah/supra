<template>
  <div class="index">
    <div class="banner">
      <p>Corrugated Box Manufacturer</p>
      <p>Export Quality Box</p>
      <p class="headline">SUPRA</p>
      <p class="year">Founded in 2016</p>
    </div>
    <div class="product" id="product">
      <div class="section-title">Products</div>
      <div class="product-body">
        <div class="product-box">
          <div class="product-detail">
            <img src="/box-product1.png" alt="box-product" class="box-border" />
            <div class="product-name">Corrugated Box</div>
          </div>
          <div class="product-detail">
            <img src="/box-product1.png" alt="box-product" class="box-border" />
            <div class="product-name">Corrugated Box</div>
          </div>
          <div class="product-detail">
            <img src="/box-product1.png" alt="box-product" class="box-border" />
            <div class="product-name">Corrugated Box</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Index",
};
</script>

<style scoped>
.banner {
  width: 100%;
  position: relative;
  background: url(/box.jpg) no-repeat center;
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
  padding: 2.5%;
  letter-spacing: 0.25em;
  font-weight: 500;
  background: #726b66;
  border-bottom: 1px solid rgba(0, 0, 0, 0.13333);
  font-size: 1.12em;
}

@keyframes typewriter {
  from {
    width: 0;
  }
  to {
    width: 50%;
  }
}

/* Product */
img.box-border {
  width: 33.33%;
  height: 100%;
  padding: 15px;
  object-fit: contain;
  border: 0.2px solid #0005;
  border-radius: 25%;
}

.product-name {
  position: absolute;
}
</style>
