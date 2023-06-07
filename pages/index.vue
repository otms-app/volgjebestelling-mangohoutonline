<template>
  <nav class="navbar navbar-dark bg-black">
    <div class="container-fluid d-flex justify-content-between">
      <div></div>
      <div class="image-container">
        <a class="text-center" href="/">
          <img
            class="centered-image"
            width="300px"
            height="94px"
            src="../images/mangohoutonline_logo.png"
            alt=""
          />
        </a>
      </div>
      <div>
        <a href="https://mangohoutonline.nl" class="btn btn-shop"
          >Terug naar de webshop</a
        >
      </div>
    </div>
  </nav>

  <!-- Banner -->

  <div class="background-image">
    <div class="overlay">
      <div class="centered-text">
        <h1>Volg je bestelling</h1>
      </div>
    </div>
  </div>

  <!-- v-if and v-else SearchFormSteps/OrderDetails -->

  <!-- Footer -->

  <div class="footer border-top">
    <div class="text-center">
      <p class="footer-p">
        &copy; {{ new Date().getFullYear() }} Mangohoutonline<br />Aan de
        informatie op onze website kunnen geen rechten worden ontleend
      </p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
/* Navbar */
.navbar {
  height: 115px;
  z-index: 1;
  padding-top: 0 !important;
}

.filler {
  width: 195.95px;
}

.image-container {
}

.btn {
  color: #fff;
}

.btn-shop {
  border-radius: 0 !important;
  right: 20px;
  background-color: rgb(187, 137, 84);
}

.btn-shop:hover {
  color: #fff;
  background-color: rgb(183, 125, 81);
}

.header {
  padding-bottom: 20px;
  padding-left: 40px;
  background: black;
  position: relative;
}

/* Banner */
.background-image {
  height: 300px;
  position: relative;
  background-size: cover;
  background-image: url(../images/banner.jpg);
}

.background-image::before {
  content: '';
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('../images/banner.jpg'); /* Replace with the actual image path */
  background-size: cover;
  background-position: center;
  z-index: -1;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(
    0,
    0,
    0,
    0.5
  ); /* Adjust the desired overlay color and opacity */
  display: flex;
  justify-content: center;
  align-items: center;
}

.centered-text {
  text-align: center;
  color: #ffffff; /* Adjust the desired text color */
  font-family: sans-serif;
  font-weight: bold;
}

.centered-image {
  max-width: 100%;
  max-height: 100%;
}

/* Footer */

.footer {
  margin-top: 15px;
  font-size: 11px;
  font-family: sans-serif;
}

.footer-p {
  margin-top: 15px;
}
</style>
