<template>
    <div class="container container-fluid container-sm">
        <div class="card border-card mb-3">
              <h5 class="card-title">Carrinho de Compras</h5>
              <div class="card-body text-dark">
                  <div class="card-body">
                    <div class="table-responsive-sm ">
                      <table class="table">
                        <thead>
                          <tr>
                            <th class="colunas" scope="col" >#</th>
                            <th class="colunas" scope="col" >Produto</th>
                            <th class="colunas" scope="col" >Preço</th>
                            <th class="colunas" scope="col" >Quantidade</th>
                            <th class="colunas" scope="col" >-</th>
                          </tr>
                        </thead>
                        <tbody class="table-group-divider-2" v-for="(produto, index) in produtos" :key="index">
                          <tr>
                            <th scope="row"><center><img :src="produto.imagem" class="card-img-top" alt="..."></center></th>
                            <td><center>{{produto.nome}}</center></td>
                            <td><center>{{produto.valor}}</center></td>
                            <td>    
                              <div class="input-groupe">
                                <div class="input-quant"><center>
                                    <button @click="incrementaQuantidade(index)" type="button" class="btn"
                                        style="--bs-btn-padding-y: .25rem; --bs-btn-padding-x: .5rem; --bs-btn-font-size: .75rem;">
                                    <i class="pi pi-arrow-up" style="font-size: 1.0rem"></i>
                                    </button>
                                    <input v-model="produto.quantidade" class="text-input"style="width: 70px;" type="number" min="1">
                                    <button @click="diminuiQuantidade(index)" type="button" class="btn "
                                        style="--bs-btn-padding-y: .25rem; --bs-btn-padding-x: .5rem; --bs-btn-font-size: .75rem;">
                                    <i class="pi pi-arrow-down" style="font-size: 1.0rem"></i>
                                    </button></center>
                                </div>
                              </div>
                            </td>
                            <td>
                              <center>
                              <button @click="removerProduto(index)"type="button" class="btn btn-danger"
                                style="--bs-btn-padding-y: .25rem; --bs-btn-padding-x: .5rem; --bs-btn-font-size: .75rem;">
                                <i class="pi pi-trash" style="font-size: 1.0rem"></i>
                              </button>
                            </center>
                            </td>
                          </tr>
                        </tbody>
                      </table>
                    </div>
                  </div>
              </div>
        </div>
        <div class="position-cards">
          <div class="card text-bg-secondary mb-3" style="max-width: 28rem; color: black !important;  ">
                <div class="card-title" style="font-size: 1.5rem; color: green;">Resumo da compra</div>
                <hr></hr>
                  <div class="card-body" style="color: white;">
                    <div class="table-responsive-sm ">
                      <table class="table">
                        <thead>
                          <tr>
                            <th class="text-buy" scope="col">Total</th>
                            <th class="text-buy" scope="col">{{total}}</th>
                          </tr>
                        </thead>
                        <tbody>
                          <th class="text-buy" scope="col">Frete</th>
                          <th class="text-buy" scope="col">Gratuito</th>
                        </tbody>  
                      </table>
                    </div>
                    <div class="table-responsive-sm">
                      <table class="table">
                        <thead>
                          <tr>
                            <th class="text-buy" scope="col">Calcular Frete</th>
                          </tr>
                        </thead>
                      </table>
                    </div>
                    <tbody class="table-group-divider">
                      <th scope="row"></th>
                      <th class="text-buy2" scope="col">
                        <div class="input-group mb-3">
                      <input type="text" class="form-control" placeholder="_____-___" aria-label="Recipient's username" aria-describedby="button-addon2">
                      <button class="btn btn-success" type="button" id="button-addon2">Calcular</button>
                    </div>  
                      </th>
                    </tbody>
                      <router-link><a style="color: green; ">Adicionar Cupom</a></router-link>
                    <center><a href="#" class="btn btn-success" style="width: 20rem; margin-top: 80px; ">Finalizar Compra</a></center>
                  </div>
              </div>
            </div>
    </div>
    </template>
    
    <script>
     export default{
      data(){
        return{
          produtos: [
            {imagem: '/favicon.ico', nome: 'Mouse Logitech Pro', valor: 'R$800,00', quantidade: 1}
          ],
          total: 'R$ 2100,00',
        };
      },
      //Splice **Remove produto**
      methods: {
          incrementaQuantidade(index){
            this.produtos[index].quantidade++; 
          },
          diminuiQuantidade(index){
            if (this.produtos[index].quantidade >= 1 )
            {
              this.produtos[index].quantidade--;
            }
            else if (this.produto[index].quantidade == 0){
              this.produtos.splice(index, 1); 
            }
          },
          removerProduto(index){
            this.produtos.splice(index,1); 
          },
        },
     };
    </script>
    
    <style scoped>
    .container {
      display: flex;
      flex-wrap: wrap;
      width: 100%;
      height: 100vh;
      border: none;
    }
    .img-main {
      background-color: rgba(19, 35, 47, 0.9);
      justify-content: center;
    }
    .card {
      justify-content: center;
      width: 80rem;
      border-color: #eeeeee;
      box-sizing: border-box;
      border-radius: 1.3rem;
    }
    b {
      color: #34e7f8;
    }
    .card-title {
      color: #34e7f8;
      text-align: center;
      font-size: 2rem;
      background-color: white;
      border-radius: 20px;
    }
    .text-bg-secondary {
      background-color: white !important;
    }
    .card-text {
      color: #34e7f8;
    }
    .card.border-card.mb-3 {
      width: 50rem;
    }
    .position-cards .card {
      display: flex;
      flex-wrap: wrap;
      width: auto;
      position: static;
      padding: 12px;
      border: none;
    }
    .card-img-top {
      width: 50px;
    }
    .card.text-bg-secondary.mb-3 {
      left: 50px;
    }
    body {
      background-color: white;
    }
    .colunas {
      text-align: center;
    }
    .text-input {
      text-align: center;
      border-radius: 10px;
      border-color: #dee2e6;
      border-style: solid;
    }
    .text-buy {
      text-align: center;  
      color: black;
    }
    
    </style>