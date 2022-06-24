<script setup lang="ts">
import TheWelcome from '@/components/TheWelcome.vue'
import NavBar from '@/components/NavBar.vue'
import SideNav from '@/components/SideNav.vue'
</script>

<template>
<NavBar />
<section class="principal-container-sesion">
  <SideNav />
    <div class="info-user-container" >
      <div class="" style="width: 95%;">
        <p class="">21 de Abril, 2022</p>
        <p class="text-xl">Bienvenida, Xenna</p>
      </div>
      <div class="flex flex-col p-md mt-lg text-center box-shadow-container text-blue-primary">
        <i class="fa-solid fa-circle-info self-right"></i>
        <p class="text-lg ">Periodo actual</p>
        <p class="text-lg pb-md">01 al 15 de agosto</p>
        <div style="width: 350px;">
          <div class="semi-donut " style="--percentage : 80; --fill: #00e097 ;margin-left: 22px;">
            <div class="flex flex-col text-blue-primary" style="padding-right:40px;padding-bottom: 20px;">
              <span class="text-xl">$3,400</span>
              <span class="text-md font-lighter">Disponible</span>
            </div>
          </div>
        </div>
        <div class="w-full flex justify-between mt-md">
          <p>Inicia Periodo</p>
          <div>
            <p>13 de Agosto</p>
            <p>Fecha de corte</p>
          </div>
        </div>
        <div class="mt-md">
          <button class="button-graph">Retirar un monto</button>
        </div>
      </div>
      <div class="">
        <p>Caja 2</p>
      </div>
      <div class="">
        <p>Caja 3</p>
      </div>
    </div>
</section>
</template>


<style>
.principal-container-sesion{
  display: flex;
  justify-content: space-between;
}


.box-shadow-container{
  width: 400px;
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  border-radius: 10px;
}


.info-user-container{
    width: 90%;
    display: flex;
    justify-content: initial;
    flex-direction: column;
    align-items: center;
    padding-top: 32px;

}


.button-graph{
    height: 45px;
    width: 200px;
    background-color: #2565c7;
    color: #fff;
    border: 0;
    border-radius: 20px;
    padding-left: 10px;
    padding-right: 10px;

}


 .semi-donut {
	 --percentage: 0;
	 --fill: #ff0;
	 width: 400px;
	 height: 150px;
	 position: relative;
	 color: #fff;
	 font-size: 22px;
	 font-weight: 600;
	 overflow: hidden;
	 color: var(--fill);
	 display: flex;
	 align-items: flex-end;
	 justify-content: center;
	 box-sizing: border-box;
}
 .semi-donut:after {
	 content: '';
	 width: 350px;
	 height: 350px;
	 border: 50px solid;
	 border-color: rgba(0, 0, 0, 0.15) rgba(0, 0, 0, 0.15) var(--fill) var(--fill);
	 position: absolute;
	 border-radius: 50%;
	 left: 0;
	 top: 0;
	 box-sizing: border-box;
	 transform: rotate(calc(1deg * ( -45 + var(--percentage) * 1.8 )));
	 animation: fillAnimation 1s ease-in;
}
 .semi-donut-model-2 {
	 width: 300px;
	 height: 150px;
	 position: relative;
	 text-align: center;
	 color: #fff;
	 font-size: 22px;
	 font-weight: 600;
	 border-radius: 150px 150px 0 0;
	 overflow: hidden;
	 color: var(--fill);
	 display: flex;
	 align-items: flex-end;
	 justify-content: center;
	 box-sizing: border-box;
}
 .semi-donut-model-2:before, .semi-donut-model-2:after {
	 content: '';
	 width: 300px;
	 height: 150px;
	 border: 50px solid var(--fill);
	 border-top: none;
	 position: absolute;
	 transform-origin: 50% 0% 0;
	 border-radius: 0 0 300px 300px;
	 box-sizing: border-box;
	 left: 0;
	 top: 100%;
}
 .semi-donut-model-2:before {
	 border-color: rgba(0, 0, 0, .15);
	 transform: rotate(180deg);
}
 .semi-donut-model-2:after {
	 z-index: 3;
	 animation: 1s fillGraphAnimation ease-in;
	 transform: rotate(calc(1deg * ( var(--percentage) * 1.8 )));
}
 .semi-donut-model-2:hover:after {
	 opacity: 0.8;
	 cursor: pointer;
}
 .multi-graph {
	 width: 300px;
	 height: 150px;
	 position: relative;
	 color: #fff;
	 font-size: 22px;
	 font-weight: 600;
	 display: flex;
	 align-items: flex-end;
	 justify-content: center;
	 overflow: hidden;
	 box-sizing: border-box;
}
 .multi-graph:before {
	 content: '';
	 width: 300px;
	 height: 150px;
	 border: 50px solid rgba(0, 0, 0, .15);
	 border-bottom: none;
	 position: absolute;
	 box-sizing: border-box;
	 transform-origin: 50% 0%;
	 border-radius: 300px 300px 0 0;
	 left: 0;
	 top: 0;
}
 .multi-graph .graph {
	 width: 300px;
	 height: 150px;
	 border: 50px solid var(--fill);
	 border-top: none;
	 position: absolute;
	 transform-origin: 50% 0% 0;
	 border-radius: 0 0 300px 300px;
	 left: 0;
	 top: 100%;
	 z-index: 5;
	 animation: 1s fillGraphAnimation ease-in;
	 transform: rotate(calc(1deg * ( var(--percentage) * 1.8 )));
	 box-sizing: border-box;
	 cursor: pointer;
}
 .multi-graph .graph:after {
	 content: attr(data-name) ' ' counter(varible) '%';
	 counter-reset: varible var(--percentage);
	 background: var(--fill);
	 box-sizing: border-box;
	 border-radius: 2px;
	 color: #fff;
	 font-weight: 200;
	 font-size: 12px;
	 height: 20px;
	 padding: 3px 5px;
	 top: 0px;
	 position: absolute;
	 left: 0;
	 transform: rotate(calc(-1deg * var(--percentage) * 1.8)) translate(-30px, 0px);
	 transition: 0.2s ease-in;
	 transform-origin: 0 50% 0;
	 opacity: 0;
}
 .multi-graph .graph:hover {
	 opacity: 0.8;
}
 .multi-graph .graph:hover:after {
	 opacity: 1;
	 left: 30px;
}
 @keyframes fillAnimation {
	 0% {
		 transform: rotate(-45deg);
	}
	 50% {
		 transform: rotate(135deg);
	}
}
 @keyframes fillGraphAnimation {
	 0% {
		 transform: rotate(0deg);
	}
	 50% {
		 transform: rotate(180deg);
	}
}
 





</style>
