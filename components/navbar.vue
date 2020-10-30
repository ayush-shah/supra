<template>
  <nav>
    <ul>
      <li>
        <nuxt-link to="/">SUPRA <sub>PACKAGING</sub></nuxt-link>
      </li>
      <li><nuxt-link to="#">HOME</nuxt-link></li>
      <li><nuxt-link to="#product">PRODUCTS</nuxt-link></li>
      <li><nuxt-link to="#about">ABOUT US</nuxt-link></li>
      <li><nuxt-link to="#contact">CONTACT US</nuxt-link></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  mounted: () => {
    window.onscroll = () => {
      if (
        document.body.scrollTop >
          document.getElementsByTagName("nav")[0].scrollHeight ||
        (document.documentElement.scrollTop >
          document.getElementsByTagName("nav")[0].scrollHeight &&
          document
            .getElementsByTagName("nav")[0]
            .classList.contains("fixedNav"))
      ) {
      } else if (
        document.body.scrollTop >
          document.getElementsByTagName("nav")[0].scrollHeight ||
        document.documentElement.scrollTop >
          document.getElementsByTagName("nav")[0].scrollHeight
      ) {
        document.getElementsByTagName("nav")[0].classList.add("fixedNav");
      } else {
        document.getElementsByTagName("nav")[0].classList.remove("fixedNav");
      }
    };
  },
};
</script>

<style scoped>
ul {
  list-style: none;
  display: flex;
  padding: 0;
  margin: 0;
  flex: 1 0 100%;
  flex-flow: row wrap;
}

li:nth-child(1) {
  margin-right: auto;
  font-size: 1.2em;
  font-weight: 600;
  letter-spacing: 0.125em;
}
li:hover {
  text-shadow: none;
}
li {
  margin: 0 2.5%;
  font-size: 0.8em;
  font-weight: 300;
  align-self: center;
  transition: 0.25s all ease-in-out;
  text-shadow: 2px 2px 0px #0005;
}
nav li sub {
  font-size: 0.6em;
}
nav {
  transition: all 0.5s ease-in-out;
  position: fixed;
  left: 0;
  top: 0;
  padding: 0 1.5%;
  width: 100%;
  background: #29252257;
  z-index: 4;
  height: 10vh;
  display: flex;
}
nav.fixedNav {
  height: 8vh;
  background: #fffe;
  box-shadow: 0px 1px 10px 0px #0005;
}
nav.fixedNav a {
  color: #000;
  text-shadow: none;
}

nav.fixedNav li:hover {
  text-decoration: underline dotted;
}
</style>