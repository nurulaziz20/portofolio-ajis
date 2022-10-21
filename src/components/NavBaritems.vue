<script></script>

<template>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark p-7">
    <div class="container">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
    >
        <span class="navbar-toggler-icon"></span>
      </button>

      <nav class="nav navbar-right navbar-expand-lg navbar-dark bg-dark   ">
  <a class="navbar-brand" href="#">Portofolio</a>
</nav>

      <div class="nav navbar-right collapse navbar-collapse " id="navbarSupportedContent">
        <ul class="nav navbar-nav navbar-right">
          <li class="nav-item">
            <a class="nav-link " aria-current="page" href="#"
              ><RouterLink to="/">Home</RouterLink></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"
              ><RouterLink to="/about">About</RouterLink></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"
              ><RouterLink to="/contact">Contact</RouterLink></a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style>
.navbar {
  background-color: white;
  margin-bottom: 50px;
  border-bottom: 1px solid black;
  margin: auto;
  position: flex;
}
li a {
  color: black;
  font-size: 18px;
  text-decoration: none;

}


</style>