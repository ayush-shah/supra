<template>
  <div class="product-lineup">
    <div class="prod">
      <div class="prod-productbox">
        <div class="prod-img">
          <img src="/supra/box03.jpg" alt="" />
        </div>
        <div class="prod-desc">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis,
          voluptatem natus odio mollitia eaque possimus commodi sequi. Nostrum
          molestiae sint eius in cum repellendus quis quasi sed quam, harum
          voluptates?
        </div>
      </div>
      <div class="prod-productbox">
        <div class="prod-img">
          <img src="/supra/box03.jpg" alt="" />
        </div>
        <div class="prod-desc">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis,
          voluptatem natus odio mollitia eaque possimus commodi sequi. Nostrum
          molestiae sint eius in cum repellendus quis quasi sed quam, harum
          voluptates?
        </div>
      </div>
      <div class="prod-productbox">
        <div class="prod-img">
          <img src="/supra/box03.jpg" alt="" />
        </div>
        <div class="prod-desc">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis,
          voluptatem natus odio mollitia eaque possimus commodi sequi. Nostrum
          molestiae sint eius in cum repellendus quis quasi sed quam, harum
          voluptates?
        </div>
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
.product-lineup {
  display: flex;
  position: relative;
  border-radius: 15px;
  flex-flow: column wrap;
}
.prod {
  position: relative;
  background: url("/supra/box04.jpg") no-repeat;
  min-height: 100vh;
  height: auto;
  background-attachment: fixed;
  background-size: cover;
}
.prod::before {
  content: "";
  border-radius: 0px 10px 0 10px;
  position: absolute;
  left: 50%;
  top: 50%;
  width: 90vh;
  backdrop-filter: blur(10px);
  height: 90vh;
  background: #fff5;
  transform: translate(-50%, -50%);
}

.prod-img img {
  object-fit: cover;
  width: 100%;
  -o-object-position: center;
  object-position: center;
  top: -10%;
  left: -10%;
  height: 120%;
  box-shadow: 0px 0px 5px 6px rgba(0, 0, 0, 0.33333);
  position: relative;
  display: block;
}
.prod-productbox {
  position: relative;
  display: flex;
  width: 90vh;
  height: calc(90vh / 3);
  margin: auto;
  top: 5vh;
}

.prod-img {
  position: relative;
  flex: 1 0 45%;
}

.prod-desc {
  flex: 1 0 55%;
  color: #fff;
  height: 100%;
  font-size: 0.9em;
  position: relative;
  width: 100%;
  display: flex;
  padding-right: 20px;
  margin-left: auto;
  align-items: center;
}
.prod-productbox:nth-child(even) {
  flex-flow: row-reverse;
}
.prod-productbox:nth-child(even) .prod-img img {
  left: 10%;
}
.prod-productbox:nth-child(even) .prod-desc {
  margin-left: unset;
  text-align: right;
  margin-right: unset;
  padding-left: 20px;
  padding-right: 0;
}
@media screen and (max-width: 480px) {
  .prod::before {
    width: 90vw;
    height: 90vh;
  }
  .prod {
    width: 100%;
  }
  .prod-productbox {
    height: 30vh;
    width: 90%;
    flex-flow: column wrap;
  }
  .prod-img {
    position: relative;
    flex: 1 0;
    height: 60%;
    width: 100%;
  }
  .prod-img img {
    width: 100%;
    left: 0%;
    top: 0%;
    height: 100%;
  }
  .prod-productbox:nth-child(even) {
    flex-flow: column wrap;
  }
  .prod-productbox:nth-child(even) .prod-img img {
    left: 0%;
  }
  .prod-desc {
    font-size: 3vw;
    flex: 1 0;
    text-align: center;
    padding: unset;
    height: 50%;
    width: 100%;
  }
  .prod-productbox:nth-child(even) .prod-desc {
    text-align: center;
    padding: unset;
  }
  .prod-productbox:first-child .prod-img img {
    border-top-right-radius: 10px;
  }
}
</style>