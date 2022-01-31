<template>
   <div id="nav">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse  navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav nav-menu me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">
                   <router-link to="/">Home</router-link>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <router-link to="/products">
                    Produtos
                </router-link>               
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                 ZoneMuzik
              </a>              
            </li>
            <li class="nav-item">
              <a class="nav-link">
                 <router-link to="/about">Encomenda</router-link>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link"  href="#">
                 Fale Conosco
              </a>
            </li>
          </ul>
          <form class="d-flex ml-5">
            <ul class="navbar-nav">
                <li class="nav-item">
                  <a class="nav-link" href="#">
                  <i class="fas fa-phone-alt">             
                  </i> +244 9234 323 244 </a>
                </li>
                <li class="nav-item"><a class="nav-link" href="#"><i class="fab fa-facebook"></i></a></li>
                <li class="nav-item"><a class="nav-link" href="#"><i class="fab fa-instagram"></i></a></li>
                <li class="nav-item"><a class="nav-link" href="#"><i class="fab fa-twitter"></i></a></li>
                <li class="nav-item"><a class="nav-link" href="#"><i class="fab fa-whatsapp"></i></a></li>
                <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" href="#" id="navbarScrollingDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                 Login
                </a>
                <ul class="dropdown-menu ml-5" aria-labelledby="navbarScrollingDropdown">
                  <li><a class="dropdown-item" href="#">Editar Perfil</a></li>                  
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Sair</a></li>
                </ul>
              </li>
            </ul>
          </form>
        </div>
      </div>
    </nav> 
    <app-publicidades/> 
    <router-view/>
    <app-rodape>
    </app-rodape>         
    </div>
    
</template>
<script>
import Publicidades from './components/Publicidades.vue';
import Rodape from './components/Rodape.vue';

export default {
  name: 'App',
  components: {
    'app-publicidades': Publicidades,
    'app-rodape': Rodape,
  },   
};
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Tangerine:wght@700&display=swap');
.nav-menu {
   color: white;
    font-size: 20pt;
    font-family: 'Tangerine', cursive;
} 
.nav-menu a{
  color: rgb(197, 192, 192);
  text-decoration: none;
  font-size: 25pt;
}

.nav-menu a:hover{
  color: rgb(225, 227, 231);
  transition: 0.5s;
}

</style>
