<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
<nav>
  <div>
      <i class="fa-solid fa-bell"></i>
      <i class="fa-solid fa-bars display-hamburger-menu"></i>
  </div>
</nav>
</template>

<style scoped>
  
nav{
  background-color: #2565c7;
  height: 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding: 0 16px ;
}

nav div i{
 color: white;
}

nav div i:first-child{
 margin-right: 16px;
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

 .movile-none {
    display: none;
  }


/*   nav {

  } */
}

@media (min-width: 1024px) {

  .desktop-none{
    display: none;
  }



}
</style>
