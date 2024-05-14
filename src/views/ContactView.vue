<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <div class="form-wrapper">
            <div class="title"><h1>Entre em contato conosco</h1></div>
            <hr class="line-title">
            <div v-if="showMessage" class="alert alert-success" role="alert">
              Mensagem enviada com sucesso! Entraremos em contato em breve.
            </div>
            <div class="mb-3">
              <label for="exampleFormFirstName" class="form-label">Primeiro Nome</label>
              <input type="name" class="form-control" placeholder="Primeiro nome" aria-label="First name" v-model.trim="formData.firstName">
              <span v-if="errors.firstName" class="error">{{ errors.firstName }}</span>
            </div>
            <div class="mb-3">
              <label for="exampleFormLastName" class="form-label">Sobrenome</label>
              <input type="last-name" class="form-control" placeholder="Sobrenome" aria-label="Last name" v-model.trim="formData.lastName">
              <span v-if="errors.lastName" class="error">{{ errors.lastName }}</span>
            </div>
            <div class="mb-3">
              <label for="exampleFormControlInput1" class="form-label">E-mail</label>
              <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="nome@exemplo.com" v-model.trim="formData.email">
              <span v-if="errors.email" class="error">{{ errors.email }}</span>
            </div>
            <div class="mb-3">
              <label for="exampleFormSelect" class="form-label">Assunto</label>
              <select class="form-select" aria-label="Default select example" v-model="formData.subject">
                <option selected>Assunto</option>
                <option value="1">Reembolso</option>
                <option value="2">Previsão de entrega</option>
                <option value="3">Dúvidas/Reclamações</option>
              </select>
              <span v-if="errors.subject" class="error">{{ errors.subject }}</span>
            </div>
            <div class="mb-3">
              <label for="exampleFormControlTextarea1" class="form-label">Mensagem</label>
              <textarea class="form-control" id="exampleFormControlTextarea1" rows="3" v-model.trim="formData.message"></textarea>
              <span v-if="errors.message" class="error">{{ errors.message }}</span>
            </div>
            <button @click="submit" class="btn btn-primary">Enviar</button>
          </div>
        </div>
        <div class="col-md-6">
          <img src="/src/assets/images/contact.svg" alt="" class="img-fluid">

          <div class="card mt-4" style="width: 23rem;">
            <div class="card-header"><b>Suporte por telefone</b></div>
            <ul class="list-group list-group-flush">
              <li class="list-group-item">Telefone: (14) 998877665</li>
              <li class="list-group-item"><b>Horários de funcionamento:</b></li>
              <li class="list-group-item">Segunda a Sexta: 8:00 - 18:00</li>
              <li class="list-group-item">Sábado: 09:00 - 15:00</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import { onMounted, reactive, ref } from 'vue';

const formData = reactive({
  firstName: '',
  lastName: '',
  email: '',
  subject: '',
  message: ''
});

const errors = reactive({
  firstName: null,
  lastName: null,
  email: null,
  subject: null,
  message: null
});

const showMessage = ref(false); 

const validateForm = () => {
  let valid = true;
  
  if (!formData.firstName.trim()) {
    errors.firstName = "Por favor, insira seu primeiro nome";
    valid = false;
  } else {
    errors.firstName = null;
  }

  if (!formData.lastName.trim()) {
    errors.lastName = "Por favor, insira seu sobrenome";
    valid = false;
  } else {
    errors.lastName = null;
  }

  const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  if (!formData.email.trim() || !emailRegex.test(formData.email)) {
    errors.email = "Por favor, insira um endereço de e-mail válido";
    valid = false;
  } else {
    errors.email = null;
  }

  if (formData.subject === 'Assunto') {
    errors.subject = "Por favor, selecione um assunto";
    valid = false;
  } else {
    errors.subject = null;
  }

  if (!formData.message.trim()) {
    errors.message = "Por favor, insira uma mensagem";
    valid = false;
  } else {
    errors.message = null;
  }

  return valid;
};

const submit = () => {
  if (validateForm()) {
    console.log("Formulário válido, enviando...");
    showMessage.value = true;
  } else {
    console.log("Formulário inválido");
  }
};
</script>

<style scoped>

</style>
