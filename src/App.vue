<script setup>
import {ref} from 'vue'

let num = ref(0)

</script>
<template>

<nav class="navbar navbar-expand-lg navbar-dark border-bottom border-body">
  <div class="container-fluid">
    <router-Link class="navbar-brand" to="/"><h1 class="logo">VIMA<span>STORE</span></h1></router-Link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <router-Link class="nav-link" aria-current="page" to="/">Inicio</router-Link>
        </li>
        <li class="nav-item">
          <router-Link class="nav-link" aria-current="page" to="/about">Sobre</router-Link>
        </li>
        <li class="nav-item">
          <router-Link class="nav-link" aria-current="page" to="/contact">Contato</router-Link>
        </li>
      </ul>
    </div>
  </div>
</nav>
<div class="main">
  <router-view></router-view>
</div>

<footer class="text-light">
  <div>
    Unimar | ADS | {{ new Date().getFullYear() }}
  </div>
</footer>

</template>
<style>


.navbar {
  background-color: #00474F;
}

footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
  background-color: #00474F;
}



</style>