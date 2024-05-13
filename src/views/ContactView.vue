<script setup>
import { onMounted, reactive, ref } from 'vue';


</script>

<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <div class="form-wrapper">
            <div class="title"><h1>Entre em contato conosco</h1></div>
            <hr class="line-title">
            <div class="mb-3">
              <label for="exampleFormFirstName" class="form-label">Primeiro Nome</label>
              <input type="name" class="form-control" placeholder="Primeiro nome" aria-label="First name">
            </div>
            <div class="mb-3">
              <label for="exampleFormLastName" class="form-label">Sobrenome</label>
              <input type="last-name" class="form-control" placeholder="Sobrenome" aria-label="Last name">
            </div>
            <div class="mb-3">
              <label for="exampleFormControlInput1" class="form-label">E-mail</label>
              <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="nome@exemplo.com">
            </div>
            <div class="mb-3">
              <label for="exampleFormSelect" class="form-label">Assunto</label>
              <select class="form-select" aria-label="Default select example">
                <option selected>Assunto</option>
                <option value="1">Reembolso</option>
                <option value="2">Previsão de entrega</option>
                <option value="3">Dúvidas/Reclamações</option>
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

</style>
