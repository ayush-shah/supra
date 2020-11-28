<template>
  <div class="product-box">
    <div class="product-detail">
      <img src="box-product1.png" alt="box-product" class="box-border" />
      <div class="product-wrapper">
        <p>Corrugated Box</p>
        <ul>
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
</template>

<script>
export default {
  name: "ProductBox",
};
</script>

<style scoped>
.product-detail {
  position: relative;
  display: flex;
  width: 100%;
  flex-wrap: nowrap;
}
.product-detail:nth-child(even) {
  flex-direction: row-reverse;
}

.product-wrapper {
  width: 0;
  flex: 0 1;
  visibility: hidden;
  overflow: hidden;
  transition: 1s all;
  white-space: nowrap;
  align-content: center;
  margin: 5%;
  display: flex;
  flex-flow: column wrap;
}
.product-wrapper > * {
  margin:0;
  padding: 0 2.5%;
}
.product-detail:hover .product-wrapper {
  width: 90%;
  visibility: visible;
  flex: 1 0;
}
img.box-border {
  box-shadow: 0px 0px 5px #0005;
  flex: 0 1 45%;
  width: 45%;
  padding: 0.5%;
  height: 250px;
  margin: 2.5%;
  transition: 1s all;
  object-fit: contain;
}
</style>