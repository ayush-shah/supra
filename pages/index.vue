<template>
  <div class="index">
    <div class="banner">
      <p>Corrugated Box Manufacturer</p>
      <p>Export Quality Box</p>
      <p class="headline">SUPRA</p>
      <p class="year">Founded in 2016</p>
    </div>
    <div class="product" id="product">
      <div class="section-title">Our Products</div>
      <div class="product-body">
        <div class="product-box">
          <div class="product-detail">
            <img src="box-product1.png" alt="box-product" class="box-border" />
            <div class="product-wrapper">
              <p>Corrugated Box</p>
              <ul>
                <li><p>3 ply</p></li>
                <li><p>3 ply</p></li>
                <li><p>3 ply</p></li>
                <li><p>3 ply</p></li>
              </ul>
            </div>
          </div>
          <div class="product-detail">
            <img src="box-product2.jpg" alt="box-product" class="box-border" />
            <div class="product-wrapper">
              <p>Corrugated Box</p>
              <ul>
                <li><p>3 ply</p></li>
              </ul>
            </div>
          </div>
          <div class="product-detail">
            <img src="box-product3.jpg" alt="box-product" class="box-border" />
            <div class="product-wrapper">
              <p>Corrugated Box</p>
              <ul>
                <li><p>3 ply</p></li>
              </ul>
            </div>
          </div>
          <div class="product-detail">
            <img src="box-product4.png" alt="box-product" class="box-border" />
            <div class="product-wrapper">
              <p>Corrugated Box</p>
              <ul>
                <li><p>3 ply</p></li>
              </ul>
            </div>
          </div>
          <div class="product-detail">
            <img src="box-product5.jpg" alt="box-product" class="box-border" />
            <div class="product-wrapper">
              <p>Corrugated Box</p>
              <ul>
                <li><p>3 ply</p></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="about" id="about"></div>
    <div class="contactus" id="contactus"></div>
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
  background: url("/supra/box.jpg") no-repeat center;
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
  position: relative;
  padding: 2.5%;
  letter-spacing: 0.25em;
  font-weight: 500;
  background: #292522;
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
.product-box {
  display: flex;
  flex-flow: row wrap;
}
.product-detail {
  position: relative;
  width: 28.33%;
  flex: 0 1 28.33%;
  display: flex;
  height: 100%;
  min-height: 40vh;
  align-items: center;
  border: 1px solid rgba(0, 0, 0, 0.33333);
  padding: 1.5%;
  justify-content: space-around;
  margin: 2.5%;
  flex-flow: row wrap;
  border-radius: 15px;
}
.quick-info > div > * {
  margin: 0 5%;
}
img.box-border {
  margin-top: 10%;
  object-fit: contain;
  width: 50%;
  height: 80%;
}
.product-detail ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-flow: row wrap;
}

ul > li {
  flex: 1 0 50%;
}
.product-detail:before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 10%;
  border-top-left-radius: 15px;
  width: 100%;
  background: #a08d70;
  border-top-right-radius: 15px;
}
.product-wrapper p {
  padding: 0;
  margin: 0;
}

/* Responsive */
@media screen and (max-width: 480px) {
  .banner {
    height: 90vh;
  }
  .banner:before {
    height: 90vh;
  }
  .product-detail {
    width: 100%;
    flex: 0 1 100%;
  }
  .product-body {
    margin-bottom: 15%;
  }
}
</style>
