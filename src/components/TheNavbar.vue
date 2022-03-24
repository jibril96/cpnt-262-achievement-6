<template>
  <div class="navbar">
  <a class="home" href="#">Home</a>
  <a href="#">Search</a>
  <a href="#">Contact</a>
  <a href="#">Login</a>
</div>
</template>

<style>
.navbar {
  width: 100%;
  background-color: #555;
  overflow-y: hidden;
  padding: 15px 0;
}

.navbar a {
  text-align: center;
  padding: 40px;
  color: rgb(0, 0, 0);
  text-decoration: none;
  font-size: 1.6rem;
}

.navbar a:hover {
  background-color: rgb(0, 47, 255);
}

.home {
  background-color: red}


@media screen and (max-width: 750px) {
  .navbar a {
    display: block;
  }
}
</style>