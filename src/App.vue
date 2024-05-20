<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark border-bottom border-body">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/"><h1 class="logo">VIMA<span>STORE</span></h1></router-link>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-auto">
          <li class="nav-item">
            <router-link class="nav-link" aria-current="page" to="/">Inicio</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" aria-current="page" to="/product">Produto-teste</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" aria-current="page" to="/contact">Contato</router-link>
          </li>
        </ul>
        <ul class="navbar-nav">
          <li class="nav-item nav-car ms-auto">
            <router-link class="nav-link" aria-current="page" to="/cart"><span class="material-symbols-outlined">shopping_cart</span></router-link>
          </li>
          <!-- <li class="nav-item nav-car ms-auto">
            <router-link class="nav-link" aria-current="page" to="/cart"><img class="cart-img" src="/src/assets/images/cart.svg"></router-link>
          </li> -->
        </ul>
      </div>
    </div>
  </nav>
  <div class="main">
    <router-view></router-view>
  </div>
</template>

<script setup>
import { ref } from 'vue';

let num = ref(0);
</script>

<style>
.logo {
  display: flex;
  align-items: center;
  color: var(--tex-color);
  font-size: 28px;
  font-weight: bold;
}

.logo i {
  color: var(--main-color);
  font-size: 32px;
  margin-right: 5px;
}

.logo {
  color: #34e7f8;
}

.logo span {
  color: #fff;
}
</style>
