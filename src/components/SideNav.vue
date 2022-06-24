<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
    <div id="side-bar" class="desktop-none movile-none ">

    <div class="side-bar-user">
      <img alt="Vue logo" class="logo" src="@/assets/images/user-photo.jpg" width="125" height="125" />

      <div>
        <p>Xenna San</p>
        <p class="pb-sm">ID. 0001234</p>
        <div>
          <p class="text-md">Monto Cash:</p>
          <div class="cost-user-container">
            <div class="coin-icon"><i class="fa-thin fa-dollar-sign"></i></div>
            <p class="text-md">$3,400</p>
          </div>
        </div>
      </div>
      <div style="align-self: end;">
        <button>Usar</button>
      </div>
    </div>
    <hr />
    <div class="side-bar-option">
      <div>
        <a href="" style="padding-left: 15px;">Menú</a>
      </div>
      <div>
         <i class="fa-solid fa-house-chimney"></i>
         <a href="">Inicio</a>
      </div>
      <div>
        <i class="fa-solid fa-clock"></i>
        <a href="">Historia</a>
      </div>
      <div>
        <i class="fa-solid fa-map"></i>
        <a href="">Guía de Uso</a>
      </div>
      <div>
        <i class="fa-solid fa-user"></i>
        <a href="">Perfil</a>
      </div>
      <div>
        <i class="fa-solid fa-file-invoice"></i>
        <a href="">Pago de Servicios</a>
      </div>
      <div>
        <i class="fa-solid fa-mobile-screen"></i>
        <a href="">Tiempo Aire</a>
      </div>
      <div>
        <i class="fa-solid fa-thumbs-up"></i>
        <a href="">Recomienda Monto</a>
      </div>
      <div>
        <i class="fa-solid fa-life-ring"></i>
        <a href="">Ayuda</a>
      </div>
      <div>
        <i class="fa-thin fa-dollar-sign"></i>
        <a href="">Acerca de Monto</a>
      </div>
      <RouterLink to="/about">
        <div>
          <i class="fa-solid fa-right-from-bracket" style="margin-top: 30px;"></i>
          <a href="">Cerrar Sesión</a>
        </div>
      </RouterLink>
    </div>

  </div>
</template>

<style scoped>
  



#side-bar{
  width: 250px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: #2565c7;
  color: white;
  padding:16px;
}

.side-bar-user{
  display: grid;
  grid-template-columns:auto auto auto;
  padding-top: 20px;
  padding-bottom: 20px;
}

.side-bar-user img{
  height: 70px;
  width: 70px;
  border-radius: 50%;
}

.side-bar-user button{
  height: 25px;
  width: 55px;
  background-color: white;
  color: #2565c7;
  border: 0;
  border-radius: 20px;
  padding-left: 10px;
  padding-right: 10px;
  
}

.side-bar-option{
  display: flex;
  flex-direction: column;
  padding-top:16px ;
}

.side-bar-option div{
  padding-top: 16px;
}

.side-bar-option div i{
   margin-right: 8px;
}

.side-bar-option a{
    color: white;
    text-decoration: none;
}

  .display-hamburger-menu {
    display: none;
  }

.coin-icon{
  height: 20px;
  width: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  background-color: #fab603;
  margin-right: 4px;
}

.cost-user-container{
  display: flex;
  justify-content: flex-start;
}

 .display-hamburger-menu {
    display: none;
  }




@media (max-width: 424px) {

  .display-hamburger-menu {
    display: inline-block;
  }

  #side-bar{
  display: none;
}






/*   nav {

  } */
}

@media (min-width: 1024px) {

 .movile-none {
    display: none;
  }



 

}
</style>
