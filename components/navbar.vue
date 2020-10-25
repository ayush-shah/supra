<template>
  <nav>
    <ul>
      <li>Supra</li>
      <li>Home</li>
      <li>Products</li>
      <li>About Us</li>
      <li>Contact Us</li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style>
ul {
  list-style: none;
  display: flex;
}

li:nth-child(1) {
  margin-right: auto;
  font-size: 1.2em;
  font-weight: 600;
}
li:hover {
  text-shadow: 1px 1px 0px rgba(0, 0, 0, 0.33333);
}
li {
  margin: 0 2.5%;
  font-size: 0.8em;
  text-transform: uppercase;
  font-weight: 300;
  transition: 0.5s all ease-in-out;
}
</style>