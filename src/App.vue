<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark border-bottom border-body">
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
            <router-Link class="nav-link" aria-current="page" to="/product">
              <span class="material-symbols-outlined">Produto-teste</span>
            </router-Link>
          </li>
          <li class="nav-item">
            <router-Link class="nav-link" aria-current="page" to="/contact">Contato</router-Link>
          </li>
          <li class="nav-item nav-car ml-auto">
          <router-Link class="nav-link" aria-current="page" to="/cart"><img class="cart-img" src="/src/assets/images/cart.svg"></router-Link>
        </li>
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
footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
}

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
