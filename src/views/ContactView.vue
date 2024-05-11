<script setup>
import { onMounted, reactive, ref } from 'vue';
let characters = reactive(ref([]));
</script>

<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <div class="form-wrapper">
            <div class="title"><h1>Entre em contato conosco</h1></div>
            <div class="mb-3">
              <label for="exampleFormFirstName" class="form-label">Primeiro Nome</label>
              <input type="text" class="form-control" placeholder="Primeiro nome" aria-label="First name">
            </div>
            <div class="mb-3">
              <label for="exampleFormLastName" class="form-label">Sobrenome</label>
              <input type="text" class="form-control" placeholder="Sobrenome" aria-label="Last name">
            </div>
            <div class="mb-3">
              <label for="exampleFormControlInput1" class="form-label">E-mail</label>
              <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
            </div>
            <div class="mb-3">
              <label for="exampleFormSelect" class="form-label">Assunto</label>
              <select class="form-select" aria-label="Default select example">
                <option selected>Assunto</option>
                <option value="1">Dúvidas</option>
                <option value="2">Dúvidas</option>
                <option value="3">Dúvidas</option>
              </select>
            </div>
            <div class="mb-3">
              <label for="exampleFormControlTextarea1" class="form-label">Texto</label>
              <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Enviar</button>
          </div>
        </div>
        <div class="col-md-6">
          <img src="/src/assets/images/contact.svg" alt="" class="img-fluid">
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.img-fluid {
  max-width: 130%; /* Define a largura máxima da imagem como 100% do seu contêiner */
  height: auto; /* Mantém a proporção da imagem */
}
</style>
