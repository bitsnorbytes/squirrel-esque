<template>
<div class="relative min-h-screen w-screen bg-slate-800">
 <div class="fixed relative top-0 left-0 right-0 flex">

     <div class="flex justify-start w-full md:w-3/4 h-[10vh] md:h-[5vh]">
     <ul class="flex items-center p-2 bg-red-600 text-3xl font-bold">
       <li class="p-2">X</li>
       <li class="p-2">Y</li>
       <li class="p-2">Z</li>
     </ul>
     <ul class="flex items-center ml-3 p-2 bg-red-600 text-3xl font-bold h-[10vh] md:h-[5vh]">
       <li class="p-2">0</li>
       <li class="p-2">0</li>
       <li class="p-2">0</li>
     </ul>  

  </div>

  <button class="evp-mobile-nav-menu-toggle block md:hidden absolute top-0 right-0 w-20 aspect-square h-[10vh] md:h-[5vh] z-50" :class="{ 'evp-mobile-nav-menu-toggle-open': ishideMenu,'evp-mobile-nav-menu-toggle-close': isShowMenu }" @click="toggleMenu"><span></span></button>
  <nav class="block flex fixed top-0 right-0 justify-start md:justify-end h-screen md:h-[5vh] md:w-1/4 z-40 md:translate-x-0 w-full ease-in-out duration-300" :class="{ 'translate-x-full':ishideMenu, 'translate-x-0': isShowMenu }">
   <ul class="absolute top-0 -right-1 z-40 md:z-0 flex flex-col h-full md:flex-row justify-center items-center py-2 px-3 bg-red-600 text-1xl font-bold">
       <li class="my-5 md:my-0 py-2 px-6 tracking-widest">HOME</li>
       <li class="my-5 md:my-0 py-2 px-6 tracking-widest">PROJECTS</li>
       <li class="my-5 md:my-0 py-2 px-6 tracking-widest">GITHUB</li>
     </ul>
     </nav> 
   
</div>
 <div class="flex flex-wrap md:flex-nowrap items-center justify-center w-full h-screen">
     <ul class="flex p-2 bg-red-600 text-3xl font-bold">
       <li class="p-2 tracking-widest">PROGRESS</li>
       <li class="p-2 tracking-widest">CODE</li>
       <li class="p-2 tracking-widest">Z</li>
     </ul>
     <ul class="flex ml-3 p-2 bg-red-600 text-3xl font-bold">
       <li class="p-2">0</li>
       <li class="p-2">2</li>
       <li class="py-2 px-1">%</li>
     </ul>  

  </div>
  </div>
</template>
<script>
export default {
  data() {
  return {
    ishideMenu: true,
    isShowMenu: false
  }
},
methods: {
toggleMenu() {
  this.isShowMenu = !this.isShowMenu;
  this.ishideMenu = !this.ishideMenu
}
}

}
</script>
<style scoped>
.evp-mobile-nav-menu-toggle-open {
background: url("../assets/icons/m-48.svg");
}
.evp-mobile-nav-menu-toggle-close {
  background: url("../assets/icons/c-50.svg");
}
.evp-mobile-nav-menu-toggle {  
  background-repeat: no-repeat;
  background-position: center;
  background-color: #dc2626;
}

</style>