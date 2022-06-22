<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
    <div id="side-bar" class="">

    <div class="side-bar-user">
      <img alt="Vue logo" class="logo" src="@/assets/images/user-photo.jpg" width="125" height="125" />

      <div>
        <p>Xenna San</p>
        <p>ID. 0001234</p>
        <div>
          <p>Monto:</p>
          <div>
            <p>Icon</p>
            <p>$3,400</p>
            <button>Usar</button>
          </div>
        </div>
      </div>
    </div>
    <div class="side-bar-option">
      <a href="">Menú</a>
      <a href="">Inicio</a>
      <a href="">Historia</a>
      <a href="">Guía de Uso</a>
      <a href="">Perfil</a>
      <a href="">Pago de Servicios</a>
      <a href="">Tiempo Aire</a>
      <a href="">Recomienda Monto</a>
      <a href="">Ayuda</a>
      <a href="">Acerca de Monto</a>
      <a href="">Cerrar Sesión</a>
    </div>

  </div>
</template>

<style scoped>
  



#side-bar{
  width: 200px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: #2565c7;
}

.side-bar-user{
  display: flex;
  justify-content: center;
  padding-top: 32px;
}

.side-bar-user img{
  height: 70px;
  width: 70px;
  border-radius: 50%;
  margin-right: 16px;
}

.side-bar-option{
  display: flex;
  flex-direction: column;
}

  .display-hamburger-menu {
    display: none;
  }

@media (hover: hover) {
  a:hover {
    background-color: hsla(160, 100%, 37%, 0.2);
  }
}

@media (max-width: 424px) {

  .display-hamburger-menu {
    display: inline-block;
  }



/*   nav {

  } */
}

@media (min-width: 1024px) {





}
</style>
