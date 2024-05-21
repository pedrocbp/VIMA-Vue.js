<script setup>
// import Navbar from '@/components/Navbar.vue';
import Button from '@/components/Button.vue';
// import Feedback from '@/components/Feedback.vue';
</script>

<template>
  <div class="">
    <Navbar />
  </div>
  <div class="container">
    <div class="row">
      <div class="col-md-8 col-sm-8 col-xs-8">
        <h2 class="title-text">DE UM NOVO ESTILO A VOCÊ</h2>
        <p class="description-text">
          Estilo sem limites, do básico ao extraordinário. Seu guarda-roupa online!
        </p>
        <div class="text-center">
          <Button />
        </div>
      </div>
      <div class="col-md-4 col-sm-4 col-xs-4">
        <img style="margin-top: 2vh; height: 40vh"
          src="https://i.pinimg.com/originals/f7/1c/5c/f71c5c1e89dbb27a7e840b6fb60932eb.png" alt="">
      </div>
    </div>
  </div>

  <div class="divisor"></div>

  <div class="text-center">
    <p class="sub-title" style="margin-bottom: 1vh;"><b>CAMISETA OVERSIZED</b></p>
  </div>
  <div class="row">
    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2022/05/camiseta-heavy-oversized-brunx-ind-roxa-4.jpg"
            alt="" />
          <h6 lass="card-title">Camiseta Heavy Oversized Brunx Ind – Roxa</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img
            src="https://brunxind.com/wp-content/uploads/2022/04/camiseta-heavy-oversized-brunx-ind-verde-floresta-4.jpg"
            alt="" />
          <h6 lass="card-title">Camiseta Heavy Oversized Brunx Ind – Verde Floresta</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2023/05/heavy-oversized-chumbo-5-1-700x1050.jpg" alt="" />
          <h6 lass="card-title">Camiseta Heavy Oversized Brunx Ind – Chumbo</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img
            src="https://brunxind.com/wp-content/uploads/2023/04/camiseta-heavy-oversized-brunx-ind-marrom-cafe-4-700x1050.jpg"
            alt="" />
          <h6 lass="card-title">Camiseta Heavy Oversized Brunx Ind – Marrom</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>
  </div>

  <div class="text-center">
    <p class="sub-title" style="margin-top: 5vh;"><b>CROPPED REGULAR</b></p>
  </div>
  <div class="row">

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2024/04/brunx-ind-cropped-regular-preto-3-700x1050.jpg"
            alt="" />
          <h6 lass="card-title">Cropped Regular Brunx Ind <br>– Preto</h6>
          <p class="product-price"> <b>R$ 49,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2024/04/brunx-ind-cropped-regular-verde-3.jpg" alt="" />
          <h6 lass="card-title">Cropped Regular Brunx Ind <br>– Verde Água</h6>
          <p class="product-price"> <b>R$ 49,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2024/04/brunx-ind-cropped-regular-rosa-3.jpg" alt="" />
          <h6 lass="card-title">Cropped Regular Brunx Ind <br>– Rosa Pink</h6>
          <p class="product-price"> <b>R$ 49,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2024/04/brunx-ind-cropped-regular-off-white-3-1.jpg"
            alt="" />
          <h6 lass="card-title">Cropped Regular Brunx Ind <br>– Off White</h6>
          <p class="product-price"> <b>R$ 49,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>
  </div>

  <div class="text-center">
    <p class="sub-title" style="margin-top: 5vh;"><b>BERMUDA</b></p>
  </div>
  <div class="row">

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2022/04/bermuda-moletom-brunx-ind-bordo-3-768x1152.jpg"
            alt="" />
          <h6 lass="card-title">Bermuda Moletom Streetwear <br>– Bordô</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2022/04/bermuda-moletom-brunx-ind-preto-3.jpg" alt="" />
          <h6 lass="card-title">Bermuda Cargo Streetwear Brunx Ind – Preta</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2024/02/bermuda-moletom-brunx-ind-marrom-2.jpg" alt="" />
          <h6 lass="card-title">Camiseta Basic Streetwear <br>– Marrom</h6>
          <p class="product-price"> <b>R$ 89,90</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>

    <div class="col text-center">
      <div class="card">
        <div class="card-body">
          <img src="https://brunxind.com/wp-content/uploads/2024/02/bermuda-moletom-brunx-ind-off-white-3.jpg" alt="" />
          <h6 lass="card-title">Bermuda Moletom Streetwear <br>– Off White</h6>
          <p class="product-price"> <b>R$ 89,99</b></p>
          <router-link class="nav-link" aria-current="page" to="/product"><a style="background-color: #212529; border: none;" href="#" class="btn btn-primary">Adicionar ao carrinho</a></router-link>
        </div>
      </div>
    </div>
  </div>

  <div class="estoque text-center">
    <div class="container text-center">
      <div class="row text-center">
        <div class="col-md-12 col-sm-12 col-xs-12">
          <h2 class="estoque-text">QUEIMA DE ESTOQUE</h2>
          <Button/>
        </div>
      </div>
      <div class="row">

      </div>
    </div>
  </div>

  <div class="page-inner-content">
    <div class="testimonials">
      <div class="testimonial">
        <p>"</p>
        <p><b>Navegação Simples e Rápida:</b> A experiência de navegação no site é intuitiva, permitindo que os usuários
          encontrem facilmente o que estão procurando.</p>
        <p class="rate">&#9733;&#9733;&#9733;&#9733;&#9733;</p>
        <p>Lucas Ribeiro</p>
      </div>
      <div class="testimonial">
        <p>"</p>
        <p><b>Design Visual Atraente:</b> O site possui um design visualmente atraente que cativa os usuários desde o
          primeiro acesso.</p>
        <p class="rate">&#9733;&#9733;&#9733;&#9733;&#9733;</p>
        <p>Felipe Araujo</p>
      </div>
      <div class="testimonial">
        <p>"</p>
        <p><b>Checkout Ágil:</b> O processo de checkout é rápido e descomplicado, proporcionando uma experiência de
          compra eficiente.</p>
        <p class="rate">&#9733;&#9733;&#9733;&#9733;&#9733;</p>
        <p>Vinicius Gazin</p>
      </div>
    </div>
  </div>
  <!-- <Feedback /> -->

</template>

<style scoped>
.container {
  background-color: rgba(0, 0, 0, 0);
  margin-top: 5vh;
}

.botao_hover

.container img {
  height: 36vh;
}

.title-text {
  font-size: 10vh;
}

.sub-title {
  font-size: 4vh;
  margin-top: 3vh;
}

.description-text {
  font-size: 2.5vh;
}

.card {
  margin-bottom: 1vh;
  width: 18.5rem;
  border: none;
  transition: all 500ms;
}


.divisor {
  background-color: #212529;
  height: 5vh;
  margin-top: 6cap;
  margin-bottom: 5vh;
}

.btn:hover {
  background-color: #212529;
}

.card img {
  height: auto;
  max-width: 30vh;
  border-radius: 1vh;
  margin-bottom: 2vh;
  margin-top: 2vh;
}

.card img:hover {
  transition: all 400ms;
  margin-bottom: 3vh;
}

.estoque {
  background-color: #212529;
  padding-top: 0.2vw;
  padding-bottom: 1vw;
  width: 100%;
  margin-bottom: 5vh;
  margin-top: 10vh;
}

.estoque-text {
  font-size: 6vw;
  color: aliceblue;
  text-align: center;
}

.testimonials{
    display: flex;
    padding: 4rem 1rem;
    justify-content: space-evenly;
}

.testimonial{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    flex-basis: 30%;
    text-align: center;
    box-shadow: 0 0 5px #afafaf;
    padding: 1rem;
    border-radius: 1rem;
    cursor: pointer;
    transition: all 0.2s;
}

.testimonial:hover{
    transform: translateY(-5px);
}

.testimonial p {
    margin: 5px 0;
}

.testimonial p:first-child{
    font-weight: bold;
    font-size: 5rem;
    color: #34e7f8;
    margin-top: 3rem;
    line-height: 2rem;
}

.testimonial p:last-child{
    font-weight: bold;
}

/* Media Queries */
@media (max-width: 800px){
    .testimonials{
        flex-direction: column;
    }

    .testimonial{
        margin-bottom: 1.2rem;
    }
}
</style>
