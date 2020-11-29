<template>
  <div class="product-box">
    <div class="product-detail">
      <img src="box-product1.png" alt="box-product" class="box-border" />
      <div class="product-wrapper">
        <p>Corrugated Box</p>
        <ul>
          <li>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magni
              non ullam ipsam deleniti voluptatibus laboriosam aut
              exercitationem doloribus. Accusantium at quasi et.
            </p>
          </li>
        </ul>
      </div>
    </div>
    <div class="product-detail">
      <img src="box-product2.jpg" alt="box-product" class="box-border" />
      <div class="product-wrapper">
        <p>Corrugated Box</p>
        <ul>
          <li>
            <p>
              blanditiis, cumque ratione velit necessitatibus iusto sapiente ut
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magni
              blanditiis, cumque ratione velit necessitatibus iusto sapiente ut
            </p>
          </li>
        </ul>
      </div>
    </div>
    <div class="product-detail">
      <img src="box-product3.jpg" alt="box-product" class="box-border" />
      <div class="product-wrapper">
        <p>Corrugated Box</p>
        <ul>
          <li>
            <p>
              non ullam ipsam deleniti voluptatibus laboriosam aut
              exercitationem doloribus. Accusantium at quasi et.
            </p>
          </li>
        </ul>
      </div>
    </div>
    <div class="product-detail">
      <img src="box-product4.png" alt="box-product" class="box-border" />
      <div class="product-wrapper">
        <p>Corrugated Box</p>
        <ul>
          <li>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magni
              blanditiis, cumque ratione velit necessitatibus iusto sapiente ut
              non ullam ipsam deleniti voluptatibus laboriosam aut
              exercitationem doloribus. Accusantium at quasi et.
            </p>
          </li>
        </ul>
      </div>
    </div>
    <div class="product-detail">
      <img src="box-product5.jpg" alt="box-product" class="box-border" />
      <div class="product-wrapper">
        <p>Corrugated Box</p>
        <ul>
          <li>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Magni
              blanditiis, cumque ratione velit necessitatibus iusto sapiente ut
              non ullam ipsam deleniti voluptatibus laboriosam aut
              exercitationem doloribus. Accusantium at quasi et.
            </p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductBox",
  mounted: () => {
    // Visibility
    // document.getElementsByClassName("product-detail").forEach((element) => {
    //   element.addEventListener("click", () => {
    //     if (!element.children[2].classList.contains("product-wrapper-open")) {
    //       document
    //         .getElementsByClassName("product-wrapper-open")
    //         .forEach((element) => {
    //           element.classList.toggle("product-wrapper-open", false);
    //         });
    //       document.getElementsByClassName("glowUp").forEach((element) => {
    //         element.classList.toggle("glowUp", false);
    //       });
    //       element.children[0].classList.toggle("glowUp");
    //       element.children[2].classList.toggle("product-wrapper-open");
    //     } else {
    //       element.children[0].classList.toggle("glowUp");
    //       element.children[2].classList.toggle("product-wrapper-open");
    //     }
    //   });
    // });
  },
};
</script>

<style scoped>
.product-detail {
  position: relative;
  display: flex;
  width: 100%;
  flex-wrap: nowrap;
  box-shadow: 0px 5px 5px 0px #0002;
}
.product-detail:nth-child(even) {
  flex-direction: row-reverse;
  text-align: right;
}
.product-detail:nth-child(even) .product-wrapper{
  align-content: flex-end;
}
.product-detail:nth-child(odd) .product-wrapper{
  align-content: flex-start;
}
.product-wrapper {
  width: 90%;
  visibility: visible;
  flex: 1 0;
  overflow: hidden;
  transition: 1s all;
  margin: 5% 0;
  display: flex;
  flex-flow: column wrap;
}
.product-wrapper > * {
  margin: 0;
  padding: 0 2.5%;
}
.product-detail:hover svg {
  fill: #0005;
}
img.box-border {
  flex: 0 1 45%;
  width: 45%;
  padding: 1.5% 0;
  height: 250px;
  margin: 2.5%;
  transition: 1s all;
  object-fit: contain;
}

ul {
  list-style-type: none;
}
@media screen and (max-width: 480px) {
  img.box-border {
    height: 125px;
    width: 125px;
    padding:2.5% 0;
    align-self:center;
  }
}
</style>