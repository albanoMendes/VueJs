<template>
    <div id="products">
        <ul class="nav nav-tabs" id="myTab" role="tablist">
            <li class="nav-item" role="presentation">
                <button class="nav-link active" id="home-tab" data-bs-toggle="tab" data-bs-target="#home" type="button" role="tab" aria-controls="home" aria-selected="true">
                    Novos Produtos
                </button>
            </li>
            <li class="nav-item" role="presentation">
                <button class="nav-link" id="profile-tab" data-bs-toggle="tab" data-bs-target="#profile" type="button" role="tab" aria-controls="profile" aria-selected="false">
                    Promoções
                </button>
            </li>
            <li class="nav-item" role="presentation">
                <button class="nav-link" id="contact-tab" data-bs-toggle="tab" data-bs-target="#contact" type="button" role="tab" aria-controls="contact" aria-selected="false">
                    Mais Vendidos
                </button>
            </li>
            <li class="nav-item" role="presentation">
                <button class="nav-link" id="buscar-tab" data-bs-toggle="tab" data-bs-target="#buscar" type="button" role="tab" aria-controls="contact" aria-selected="false">
                   <i class="fas fa-search"></i>
                </button>
            </li>
            <li class="nav-item" role="presentation">
                <button class="nav-link" id="carrinho-tab" data-bs-toggle="tab" data-bs-target="#carrinho" type="button" role="tab" aria-controls="compas-list" aria-selected="false">
                    <i class="fas fa-cart-arrow-down"></i>
                    <span>0</span>
                </button>
            </li>
        </ul>
        <div class="tab-content" id="myTabContent">
            <div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab">
                <div class="container-fluid" id="novos">
                    <div id="sub-title">
                        <h3 class="display-3">
                            <a href="#home">
                            <i class="fas fa-angle-down"></i>
                            Novos Produtos
                            </a>
                        </h3>
                        <p>Produtos disponibilizados para venda no <strong>10 Março 2022</strong></p>
                    </div>
                   <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
                        <div class="carousel-inner">
                            <div class="carousel-item active">
                                <div class="row justify-content-sm-center">

                                    <div class="col-sm-3 col-md-3 mb-5" style="width: 15rem; height: 25rem;">
                                        <div class="card card-prod">
                                        <img src="../assets/Perfume-channel-Coco-F-100ml.jpg" class="card-img-top" alt="...">
                                        <div class="card-body  desc">
                                            <h5 class="card-title">PERFUME</h5>
                                            <h6 class="card-title">Coco Channel (F) 100ml</h6>
                                            <h7 class="card-title">Preço: 6000 kz</h7><br>
                                            <label for="quantity">Qtd:</label>
                                            <input type="number" id="quantity" name="quantity" min="1" max="100" v-model="inventario.perfumes">
                                            <br><br>
                                            <a href="#" class="btn btn-outline-primary btn-ver" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom" aria-controls="offcanvasBottom">
                                            Ver
                                            <i class="fas fa-eye"></i>
                                            </a>
                                            <div class="offcanvas offcanvas-bottom centraliza" tabindex="-1" id="offcanvasBottom" aria-labelledby="offcanvasBottomLabel">
                                            <div class="offcanvas-header">
                                                <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                                            </div>
                                            <div class="container-fluid">
                                                <div class="row justify-content-between">
                                                <div class="col-md-4">
                                                    <img src="../assets/Perfume-cocoChannel(G).jpg" class="img-ver" alt="...">
                                                </div>
                                                <div class="col-md-4">
                                                    <h5 class="card-title">PERFUME</h5>
                                                    <h6 class="card-title">Coco Channel Feminino 100ml</h6>
                                                    <h7 class="card-title">Apenas: 6000 kz</h7>
                                                    <button type="button" class="btn btn-primary btn-add mt-3">
                                                    ADD  <i class="fas fa-cart-arrow-down"></i>
                                                    </button>

                                                </div>
                                                </div>
                                            </div>
                                            </div>
                                            &emsp;&emsp;
                                            <a href="#" class="btn btn-outline-primary btn-add">
                                            ADD
                                            <i class="fas fa-cart-arrow-down"></i>
                                            </a>
                                        </div>
                                        </div>
                                    </div>

                                    <div class="col-sm-3 col-md-3 mb-5" style="width: 15rem; height: 25rem;">
                                        <div class="card card-prod">
                                            <img src="../assets/Perfume-channel-Coco-F-100ml.jpg" class="card-img-top" alt="...">
                                            <div class="card-body  desc">
                                                <h5 class="card-title">PERFUME</h5>
                                                <h6 class="card-title">Coco Channel (F) 100ml</h6>
                                                <h7 class="card-title">Preço: 6000 kz</h7><br>
                                                <label for="quantity">Qtd:</label>
                                                <input type="number" id="quantity" name="quantity" min="1" max="100">
                                                <br><br>
                                                <a href="#" class="btn btn-outline-primary btn-ver" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom" aria-controls="offcanvasBottom">
                                                Ver
                                                <i class="fas fa-eye"></i>
                                                </a>
                                                <div class="offcanvas offcanvas-bottom centraliza" tabindex="-1" id="offcanvasBottom" aria-labelledby="offcanvasBottomLabel">
                                                <div class="offcanvas-header">
                                                    <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                                                </div>
                                                <div class="container-fluid">
                                                    <div class="row justify-content-between">
                                                    <div class="col-md-4">
                                                        <img src="../assets/Perfume-cocoChannel(G).jpg" class="img-ver" alt="...">
                                                    </div>
                                                    <div class="col-md-4">
                                                        <h5 class="card-title">PERFUME</h5>
                                                        <h6 class="card-title">Coco Channel Feminino 100ml</h6>
                                                        <h7 class="card-title">Apenas: 6000 kz</h7>
                                                        <button type="button" class="btn btn-primary btn-add mt-3">
                                                        ADD  <i class="fas fa-cart-arrow-down"></i>
                                                        </button>

                                                    </div>
                                                    </div>
                                                </div>
                                                </div>
                                                &emsp;&emsp;
                                                <a href="#" class="btn btn-outline-primary btn-add">
                                                ADD
                                                <i class="fas fa-cart-arrow-down"></i>
                                                </a>
                                            </div>
                                        </div>
                                    </div>

                                </div>
                            </div>
                            <div class="carousel-item">

                            </div>
                            <div class="carousel-item">

                            </div>
                        </div>
                        <button class="carousel-control-prev bt-carrosel" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Previous</span>
                        </button>
                        <button class="carousel-control-next  bt-carrosel" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Next</span>
                        </button>
                    </div>
                </div>
            </div>
            <div class="tab-pane fade" id="profile" role="tabpanel" aria-labelledby="profile-tab">
                <div class="container-fluid" id="novos">
                    <div id="sub-title">
                        <h3 class="display-3">
                            <a href="#home">
                            <i class="fas fa-angle-down"></i>
                                Promoções
                            </a>
                        </h3>
                        <p>Produtos disponibilizados para venda no <strong>10 Março 2022</strong></p>
                    </div>
                </div>

                <div id="carrosel-promocao" class="carousel slide" data-bs-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <div class="row justify-content-sm-center">

                            <div class="col-sm-3 col-md-3 mb-5" style="width: 15rem; height: 25rem;">
                                <div class="card card-prod">
                                    <img src="../assets/Shisha-Artezanal-2-Mangueiras.png" class="card-img-top" alt="...">
                                    <div class="card-body  desc">
                                        <h5 class="card-title">SHISHA</h5>
                                        <h6 class="card-title">Artezanal 2 Mangueiras</h6>
                                        <h7 class="card-title">Preço: 4000 kz</h7><br>
                                        <label for="quantity">Qtd:</label>
                                        <input type="number" id="quantity" name="quantity" min="1" max="100">
                                        <br><br>
                                        <a href="#" class="btn btn-outline-primary btn-ver" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom01" aria-controls="offcanvasBottom">
                                        Ver
                                        <i class="fas fa-eye"></i>
                                        </a>
                                        <div class="offcanvas offcanvas-bottom centraliza" tabindex="-1" id="offcanvasBottom01" aria-labelledby="offcanvasBottomLabel">
                                        <div class="offcanvas-header">
                                            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                                        </div>
                                        <div class="container-fluid">
                                            <div class="row justify-content-between">
                                            <div class="col-md-4">
                                                <img src="../assets/Shisha-Artezanal-2-Mangueiras(G).jpg" class="img-ver" alt="...">
                                            </div>
                                            <div class="col-md-4">
                                                <h5 class="card-title">SHISHA</h5>
                                                <h6 class="card-title">Artezanal 2 Mangueiras</h6>
                                                <h7 class="card-title">Apenas: 4000 kz</h7>
                                                <button type="button" class="btn btn-primary btn-add mt-3">
                                                ADD  <i class="fas fa-cart-arrow-down"></i>
                                                </button>

                                            </div>
                                            </div>
                                        </div>
                                        </div>
                                        &emsp;&emsp;
                                        <a href="#" class="btn btn-outline-primary btn-add">
                                        ADD
                                        <i class="fas fa-cart-arrow-down"></i>
                                        </a>
                                    </div>
                                </div>
                            </div>

                             <div class="col-sm-3 col-md-3 mb-5" style="width: 15rem; height: 25rem;">
                                <div class="card card-prod">
                                    <img src="../assets/Shisha-Artezanal-2-Mangueiras.png" class="card-img-top" alt="...">
                                    <div class="card-body  desc">
                                        <h5 class="card-title">SHISHA</h5>
                                        <h6 class="card-title">Artezanal 2 Mangueiras</h6>
                                        <h7 class="card-title">Preço: 4000 kz</h7><br>
                                        <label for="quantity">Qtd:</label>
                                        <input type="number" id="quantity" name="quantity" min="1" max="100" v-model="inventario.eletronicos">
                                        <br><br>
                                        <a href="#" class="btn btn-outline-primary btn-ver" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom01" aria-controls="offcanvasBottom">
                                        Ver
                                        <i class="fas fa-eye"></i>
                                        </a>
                                        <div class="offcanvas offcanvas-bottom centraliza" tabindex="-1" id="offcanvasBottom01" aria-labelledby="offcanvasBottomLabel">
                                        <div class="offcanvas-header">
                                            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                                        </div>
                                        <div class="container-fluid">
                                            <div class="row justify-content-between">
                                            <div class="col-md-4">
                                                <img src="../assets/Shisha-Artezanal-2-Mangueiras(G).jpg" class="img-ver" alt="...">
                                            </div>
                                            <div class="col-md-4">
                                                <h5 class="card-title">SHISHA</h5>
                                                <h6 class="card-title">Artezanal 2 Mangueiras</h6>
                                                <h7 class="card-title">Apenas: 4000 kz</h7>
                                                <button type="button" class="btn btn-primary btn-add mt-3">
                                                ADD  <i class="fas fa-cart-arrow-down"></i>
                                                </button>

                                            </div>
                                            </div>
                                        </div>
                                        </div>
                                        &emsp;&emsp;
                                        <a href="#" class="btn btn-outline-primary btn-add">
                                        ADD
                                        <i class="fas fa-cart-arrow-down"></i>
                                        </a>
                                    </div>
                                </div>
                            </div>

                        </div>
                    </div>
                    <div class="carousel-item">

                    </div>
                    <div class="carousel-item">

                    </div>
                </div>
                <button class="carousel-control-prev bt-carrosel01" type="button" data-bs-target="#carrosel-promocao" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next bt-carrosel01" type="button" data-bs-target="#carrosel-promocao" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
                </div>
            </div>
            <div class="tab-pane fade" id="contact" role="tabpanel" aria-labelledby="contact-tab">
                <div class="container-fluid" id="novos">
                    <div id="sub-title">
                        <h3 class="display-3">
                            <a href="#home">
                            <i class="fas fa-angle-down"></i>
                            Mais Vendidos
                            </a>
                        </h3>
                        <p>Produtos disponibilizados para venda no <strong>10 Março 2022</strong></p>
                    </div>

                    <div id="carousel-mvendidos" class="carousel slide" data-bs-ride="carousel">
                        <div class="carousel-inner">
                            <div class="carousel-item active">
                                 <div class="row justify-content-sm-center">

                                     <div class="col-sm-3 col-md-3 mb-5" style="width: 15rem; height: 25rem;">
                                        <div class="card card-prod">
                                            <img src="../assets/cigarrilha-cohiba-10.png" class="card-img-top" alt="...">
                                            <div class="card-body  desc">
                                                <h5 class="card-title">CHARUTO</h5>
                                                <h6 class="card-title">Cohiba c/10 unidades</h6>
                                                <h7 class="card-title">Preço: 25000 kz</h7><br>
                                                <label for="quantity">Qtd:</label>
                                                <input type="number" id="quantity" name="quantity" min="1" max="100">
                                                <br><br>
                                                <a href="#" class="btn btn-outline-primary btn-ver" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom02" aria-controls="offcanvasBottom">
                                                Ver
                                                <i class="fas fa-eye"></i>
                                                </a>
                                                <div class="offcanvas offcanvas-bottom centraliza" tabindex="-1" id="offcanvasBottom02" aria-labelledby="offcanvasBottomLabel">
                                                <div class="offcanvas-header">
                                                    <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                                                </div>
                                                <div class="container-fluid">
                                                    <div class="row justify-content-between">
                                                    <div class="col-md-4">
                                                        <img src="../assets/cigarrilha-cohiba-10-short-5f7246726632d-large.png" class="img-ver" alt="...">
                                                    </div>
                                                    <div class="col-md-4">
                                                        <h5 class="card-title">CHARUTO</h5>
                                                        <h6 class="card-title">Cohiba caixa com 10 unidades</h6>
                                                        <h7 class="card-title">Apenas: 25000 kz</h7>
                                                        <button type="button" class="btn btn-primary btn-add mt-3">
                                                        ADD  <i class="fas fa-cart-arrow-down"></i>
                                                        </button>

                                                    </div>
                                                    </div>
                                                </div>
                                                </div>
                                                &emsp;&emsp;
                                                <a href="#" class="btn btn-outline-primary btn-add">
                                                ADD
                                                <i class="fas fa-cart-arrow-down"></i>
                                                </a>
                                            </div>
                                        </div>
                                    </div>

                                     <div class="col-sm-3 col-md-3 mb-5" style="width: 15rem; height: 25rem;">
                                        <div class="card card-prod">
                                            <img src="../assets/cigarrilha-cohiba-10.png" class="card-img-top" alt="...">
                                            <div class="card-body  desc">
                                                <h5 class="card-title">CHARUTO</h5>
                                                <h6 class="card-title">Cohiba c/10 unidades</h6>
                                                <h7 class="card-title">Preço: 25000 kz</h7><br>
                                                <label for="quantity">Qtd:</label>
                                                <input  type="number" id="quantity" name="quantity" min="1" max="100" v-model.number="inventario.charutos">
                                                <br><br>
                                                <a href="#" class="btn btn-outline-primary btn-ver" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasBottom02" aria-controls="offcanvasBottom">
                                                Ver
                                                <i class="fas fa-eye"></i>
                                                </a>
                                                <div class="offcanvas offcanvas-bottom centraliza" tabindex="-1" id="offcanvasBottom02" aria-labelledby="offcanvasBottomLabel">
                                                <div class="offcanvas-header">
                                                    <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
                                                </div>
                                                <div class="container-fluid">
                                                    <div class="row justify-content-between">
                                                    <div class="col-md-4">
                                                        <img src="../assets/cigarrilha-cohiba-10-short-5f7246726632d-large.png" class="img-ver" alt="...">
                                                    </div>
                                                    <div class="col-md-4">
                                                        <h5 class="card-title">CHARUTO</h5>
                                                        <h6 class="card-title">Cohiba caixa com 10 unidades</h6>
                                                        <h7 class="card-title">Apenas: 25000 kz</h7>
                                                        <button type="button" class="btn btn-primary btn-add mt-3">
                                                        ADD  <i class="fas fa-cart-arrow-down"></i>
                                                        </button>

                                                    </div>
                                                    </div>
                                                </div>
                                                </div>
                                                &emsp;&emsp;                                                
                                                <button @click="addItens('charuto')" class="btn btn-outline-primary btn-add">
                                                    ADD
                                                <i class="fas fa-cart-arrow-down"></i>
                                                </button>
                                            </div>
                                        </div>
                                    </div>

                                 </div>
                            </div>
                            <div class="carousel-item">

                            </div>
                            <div class="carousel-item">

                            </div>
                        </div>
                        <button class="carousel-control-prev bt-carrosel02" type="button" data-bs-target="#carousel-mvendidos" data-bs-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Previous</span>
                        </button>
                        <button class="carousel-control-next bt-carrosel02" type="button" data-bs-target="#carousel-mvendidos" data-bs-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Next</span>
                        </button>
                    </div>
                </div>
            </div>
            <div class="tab-pane fade" id="buscar" role="tabpanel" aria-labelledby="buscar-tab">

                <nav class="navbar navbar-dark bg-dark panal-busca">
                    <form class="container-fluid">
                        <div class="input-group">
                            <input type="search" class="form-control" placeholder="ex: Perfumes Ou Baco Rabanne" aria-label="Recipient's username" aria-describedby="button-addon2">
                            <button class="btn btn-busca" type="button" id="button-addon2">
                                <i class="fas fa-search"></i>
                            </button>
                        </div>
                    </form>
                </nav>

            </div>
             <div class="tab-pane fade tab-carrinho  bg-dark text-white" id="carrinho" role="tabpanel" aria-labelledby="carrinho-tab">
                 <div id="sub-title">
                        <h3 class="display-3">
                            <a href="#home">
                            <i class="fas fa-angle-down"></i>
                             MEU CARRINHO
                            </a>
                        </h3>
                        <p>Na compra de mais de 4 produtos terá desconto de 10%, <strong>APROVEITA A PROMOÇÃO</strong> </p>
                    </div>
                 <div class="container">
                    <div class="row mb-2">
                        <table class="table table-dark text-white" id="tabela">
                            <thead>
                                <tr>
                                <th class="text-white" scope="col"></th>
                                <th class="text-white" scope="col">Nome</th>
                                <th scope="col">Tipo de Produto</th>
                                <th scope="col">Preço</th>
                                <th scope="col">Qtd</th>
                                <th scope="col">Total</th>
                                <th></th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <th scope="row">1</th>
                                    <td>Mark</td>
                                    <td>Otto</td>
                                    <td>@mdo</td>
                                    <td>@mdo</td>
                                    <td>0.0</td>
                                    <td>
                                        <a href="#">
                                            <i class="far fa-eye icon-ver"></i>
                                        </a>&emsp;
                                        <a href="#">
                                            <i class="fas fa-times icon-excluir">
                                            </i>
                                        </a>
                                    </td>
                                </tr>

                            </tbody>
                        </table>
                    </div>

                    <div class="row justify-content-center mb-5">
                        <div class="col-4">
                        Total: <span></span>
                        </div>
                        <div class="col-4">
                            <button type="button" class="btn btn-pagar mb-1">
                            Fazer Pagamento
                            </button>
                        </div>
                    </div>
                 </div>
            </div>

        </div>
    </div>
</template>
<script>
/* eslint-disable indent */
export default {
name: 'HelloWorld',
  data() {
    return {
        inventario: {
            perfumes: 0,
            eletronicos: 0,
            charutos: 0,
        },
        carrinho: {
            perfumes: 0,
            eletronicos: 0,
            charutos: 0,
        },
    };
  },
  props: {
    msg: String,
  },
  methods: {
    addItens(type) {
        this.carrinho[type] += this.carrinho[type];
      },
  },
};
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Rubik&display=swap');
.card-prod:hover{
    box-shadow: 5px 5px 5px 5px rgba(238, 234, 234, 0.788);
    transition: 0.2s;
}
.desc{
    font-size: 15pt;
    font-family: 'Rubik', sans-serif;
}
.desc input{
    width: 50px;
}
.desc{
    font-size: 15pt;
    font-family: 'Rubik', sans-serif;
}
.desc input{
    width: 100px;
}
.bt-carrosel{
    background-color: cornflowerblue;
    border-radius: 100%;
    width: 50px;
    height: 50px;
    margin-top: 25%;
}
.bt-carrosel01{
    background-color: cornflowerblue;
    border-radius: 100%;
    width: 50px;
    height: 50px;
    margin-top: 25%;
}
.bt-carrosel02{
    background-color: cornflowerblue;
    border-radius: 100%;
    width: 50px;
    height: 50px;
    margin-top: 25%;
}
.btn-ver{
    border: none;
    font-family: 'Vidaloka', serif;
}
.btn-add{
    font-family: 'Vidaloka', serif;
    background-color: rgba(16, 5, 119, 0.788);
    color: white;
    padding: 5px;
    border: none;
    border-radius: 25px;
    padding: auto 10px auto 10px
}
.btn-add:hover{
    background-color: rgb(46, 110, 230);
    color: rgba(16, 5, 119, 0.788);
    transition: 1s;
}
.btn-add i{
    color: white;
}
.card-prod{
    border: none;
    width: 500px;
    box-shadow: 2px 2px 2px 2px rgba(238, 234, 234, 0.788);
}
.centraliza {
    width: 605px;
    margin: auto auto 10% auto;
    height: 405px;
}
.img-ver{
    width: 200%;
    height: 100%;
}
#tabela th, td{
    border: none;
     padding: 20px;
     text-align: center;
     color: #fff;
}
#tabela .icon-ver{
    color: rgb(14, 17, 184);
    font-size: 12pt;
}
#tabela .icon-excluir{
    color: rgb(245, 39, 39);
    font-size: 12pt
}
#tabela .icon-ver:hover{
    color: rgb(252, 252, 252);
    transition: 0.2s;
}
#tabela .icon-excluir:hover{
    color: rgb(109, 7, 7);
     transition: 0.2s;
}
.tab-carrinho{
    font-size: 15pt;
    font-family: 'Rubik', sans-serif;
}
.tab-carrinho .btn-pagar{
    border-radius: 25px;
    background-color: rgb(10, 10, 223);
    color: white;
    font-size: 15pt;
}
.tab-carrinho .btn-pagar:hover{
    color: rgb(9, 42, 150);
    background-color: rgb(3, 3, 109);
    transition: 0.2s;
}
.panal-busca{
    padding: 10px;
    height: 100px;
}
.panal-busca input{
    background-color: rgb(24, 23, 23);
    box-shadow: 1px 1px 1px 1px rgba(63, 58, 58, 0.788);
    padding: 10px;
    text-align: center;
    border-radius: 30px;
    color: white;
    font-size: 20pt;
    font-family: 'Rubik', sans-serif;
    border: none;
}
.panal-busca input:hover {
    background-color: rgb(17, 17, 17);
    box-shadow: 2px 2px 2px 2px rgba(63, 58, 58, 0.788);
    transition: 0.5s;
}
.panal-busca .btn-busca{
    color:#fff;
    border-radius: 25px;
    border: none;
     background-color: rgb(24, 23, 23);
     font-size: 20pt;
     box-shadow: 1px 1px 1px 1px rgba(63, 58, 58, 0.788);

}
.panal-busca .btn-busca:hover{
    background-color: rgb(17, 17, 17);
    box-shadow: 2px 2px 2px 2px rgba(63, 58, 58, 0.788);
    color: rgb(118, 145, 145);
    transition: 0.5s;
}
/*.input-group{
    background-color: red;
    padding: 10px;
    width: 90%;
}
.input-group input{
    padding: 10px;
    border-radius: 25px;
    border: 1px #ffff;
    width: 80%;
    text-align: center;
}*/
</style>
