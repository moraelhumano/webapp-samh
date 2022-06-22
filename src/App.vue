<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

import NavBar from '@/components/NavBar.vue'
import SideNav from './components/SideNav.vue'
</script>

<template>


<section>
  <NavBar />
  <SideNav />

</section>
<!--  <header>
     <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />
     <div class="wrapper">
    <HelloWorld msg="You did it!" /> 

     <div class="nav">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </div>
    </div>
  </header> -->

  <RouterView />
</template>

<style>
@import '@/assets/base.css';

body{
  height: 100%;
}


</style>
