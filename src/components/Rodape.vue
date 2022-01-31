<template>
    <div class="navbar-expand-lg navbar-dark bg-dark">
        <footer class="mt-5" id="rodape">
            <div class="container navbar-expand-lg navbar-dark bg-dark">
            <div class="row justify-content-around navbar-expand-lg navbar-dark bg-dark">
                <div class="col-md-4">          
                <h6 style="margin-left:  20px;">                            
                    Paginas
                </h6>
                <ul class="nav flex-column " style="text-align: left;">
                    <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="#novos">Novos Produtos</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#promocao">Promoções</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#maisvendidos">Mais Vendidos</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#encomenda">
                        Encomenda
                    </a>
                    </li>
                </ul>
                </div>
                <div class="col-md-4">
                <h6>                            
                    Localização
                </h6>
                <h6>Luanda</h6>
                <p class="mb-1">Maianga, Marteres do Kifangodo, avanida revolução de outubro nº 46B.</p>
                <p class="mb-1">Viana, estrada do catete, zona economica n°23.</p>
                <h6>Contatos</h6>
                <p class="mb-1">TELEFONE: +222 042 567 / +222 777 993</p>
                <p class="mb-1">WHATSAPP: 999 543 455 / 923 543 455</p>
                </div>
                
                <div class="col-md-4 navbar-expand-lg navbar-dark bg-dark">
                <h6 style="text-align: center;">                                      
                    Parceiros
                </h6>
                <ul class="nav flex-column" style="text-align: center;">
                    <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="#">Overtime&NL</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#">Yebba Ent</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#">ZoneFrangace</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">
                        Os 300
                    </a>
                    </li>
                </ul>
                </div>
            </div>
            </div>
        </footer>
    </div>
</template>
<script>
export default {
    
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Vidaloka&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Tangerine:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@200&display=swap');
#rodape{
    color: white;
    font-size: 12pt;
    font-family: 'Roboto Mono', monospace;
}
#rodape h6{
    font-family: 'Vidaloka', serif;
    font-size: 16pt;
    
}
#rodape a{
    color: white;
    font-size: 20pt;
    font-family: 'Tangerine', cursive;
}
#rodape a:hover{
    color: rgb(118, 145, 145);
    transition: 2s;
    text-shadow: 1px 1px 1px 1px rgba(35, 37, 37, 0.897);
}
</style>
