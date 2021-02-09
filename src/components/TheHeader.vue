<template>
  <nav class="navbar navbar-expand-lg navbar-dark navbar-floating">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="../assets/favicon-light.png" alt="" width="40">
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarToggler" aria-controls="navbarToggler" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarToggler">
        <ul class="navbar-nav ml-auto mt-3 mt-lg-0">
          <li class="nav-item active">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/investment-packages">Investment Packages</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/faqs">FAQs</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/testimonies">Testimonies</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contact</router-link>
          </li>
        </ul>
        <div class="ml-auto my-2 my-lg-0">
          <router-link to="/login" class="btn btn-primary rounded-pill">Login</router-link>
        </div>
      </div>
    </div>
  </nav>
</template>