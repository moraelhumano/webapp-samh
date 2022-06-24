<template>

  <section class="flex justify-between sesion-container">
    <div class="sesion-container-left flex flex-col bg-blue-primary text-white pt-4xl side-bar" style="padding-left: 32px;">
      <div class="text-xl font-lighter ">
        <p>Tu dinero</p>
        <p>cuando quieras</p>
      </div>
      <p>Conoce más acerca de monto</p>
    </div>
    
    <div class="sesion-container-right pt-2xl pt-4xl" style="padding-left:32px;">
      <form class="w-fit" action="">
        <p class="text-xl">Iniciar sesión</p>
        <div class="mt-md">
          <p class="">Nombre(s)</p>
          <input class="input-form" type="text" placeholder="Ingresa tu(s) nombre(s) legal">
        </div>
        <div class="mt-md">
          <p class="">Apellido</p>
          <input class="input-form" type="text" placeholder="Ingresa tu apellido">
        </div>
        <div class="mt-md">
          <p class="">Fecha de nacimiento</p>
          <input class="input-form" type="date">
        </div>
        <div class="mt-md">
          <p class="">Correo electrónico (opcional)</p>
          <input class="input-form" type="text" placeholder="Ingresa tu correo electrónico">
        </div>
        <div class="mt-md">
          <p class="">Celular</p>
          <input class="input-form" type="text" placeholder="Ingresa tu número celular">
        </div>
        <div class="w-full flex flex-col justify-center items-center mt-md">
          <button class="button-blue">Siguiente</button>
          <button class="button-white mt-sm font-bold">Cancelar</button>
        </div>
      </form>
    </div>
  </section>
</template>

<style>

.sesion-container{
  width: 100%;
  height: 100vh;
}

.sesion-container-left{
  width: 25%;
  height: 100%;
  justify-content: space-between;
  padding-bottom: 64px;
}

.sesion-container-right{
  width: 75%;
}


.button-blue{
    height: 45px;
    width: 300px;
    background-color: #91b1e3;
    color: #fff;
    border: 0;
    border-radius: 20px;
    padding-left: 10px;
    padding-right: 10px;

}

.button-white{
    height: 45px;
    width: 300px;
    background-color: #fff;
    color: #91b1e3;
    border: 0;
    border-radius: 20px;
    padding-left: 10px;
    padding-right: 10px;

}


@media (max-width: 424px) {


  .side-bar{
  display: none;
}
}



</style>
