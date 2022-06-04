<template>
<div class="relative min-h-screen w-screen bg-slate-800">
 <div class="fixed relative top-0 left-0 right-0 flex">

     <div class="flex justify-start w-full md:w-3/4 h-[10vh]">
     <ul class="flex items-center p-2 bg-red-600 text-3xl font-bold">
       <li class="px-3 md:px-4 py-2">P</li>
       <li class="px-3 md:px-4 py-2">Y</li>
       <li class="px-3 md:px-4 py-2">S</li>
       <li class="px-3 md:px-4 py-2">L</li>
     </ul>
     <ul class="flex items-center ml-3 p-2 bg-red-600 text-3xl font-bold h-[10vh]">
       <li class="p-2">0</li>
       <li class="p-2">2</li>
       <li class="p-2">%</li>
     </ul>  

  </div>

  <button class="evp-mobile-nav-menu-toggle block md:hidden absolute top-0 right-0 w-20 aspect-square h-[10vh] z-50" :class="{ 'evp-mobile-nav-menu-toggle-open': ishideMenu,'evp-mobile-nav-menu-toggle-close': isShowMenu }" @click="toggleMenu"><span></span></button>
  <nav class="block flex fixed top-0 right-0 justify-start md:justify-end h-screen md:h-[10vh] md:w-1/4 z-40 md:translate-x-0 w-full ease-in-out duration-300" :class="{ 'translate-x-full':ishideMenu, 'translate-x-0': isShowMenu }">
   <ul class="absolute top-0 -right-1 z-40 md:z-0 flex flex-col h-full md:flex-row justify-center items-center py-2 px-3 bg-red-600 text-1xl font-bold">
       <li class="my-5 md:my-0 py-2 px-14 md:px-6 tracking-widest">HOME</li>
       <li class="my-5 md:my-0 py-2 px-14 md:px-6 tracking-widest">PROJECTS</li>
       <li class="my-5 md:my-0 py-2 px-14 md:px-6 tracking-widest">GITHUB</li>
     </ul>
     </nav> 
   
</div>
<div class="flex flex-wrap items-center justify-center w-full h-[40vh]"></div>
 <div class="flex flex-wrap content-center w-full h-[50vh] bg-red-600">
     <ul class="flex p-2 relative items-center text-6xl w-full h-[5rem] font-bold">
       <li class="p-2 flex items-center justify-end tracking-widest text-right h-full w-10/12 md:w-1/2">DEVOPS</li>
       <li class="h-full w-2/12 flex items-center justify-start"><svg xmlns="http://www.w3.org/2000/svg" width="83" height="100%" viewBox="0 0 83 97">
  <g id="Polygon_1" data-name="Polygon 1" transform="translate(83) rotate(90)" fill="#850081">
    <path d="M 88.28727722167969 78 L 8.712726593017578 78 L 48.5 9.910442352294922 L 88.28727722167969 78 Z" stroke="none"/>
    <path d="M 48.5 19.8209342956543 L 17.42548370361328 73 L 79.57451629638672 73 L 48.5 19.8209342956543 M 48.5 7.62939453125e-06 L 97 83 L 0 83 L 48.5 7.62939453125e-06 Z" stroke="none" fill="#230101"/>
  </g>
</svg>
</li>
     </ul>
     <ul class="flex p-2 relative items-center text-6xl w-full h-[5rem] font-bold">
       <li class="p-2 flex items-center justify-end tracking-widest text-right h-full w-10/12 md:w-1/2">ART</li>
       <li class="h-full w-2/12 flex items-center justify-start"><svg xmlns="http://www.w3.org/2000/svg" width="83" height="100%" viewBox="0 0 83 97">
  <g id="Polygon_2" data-name="Polygon 2" transform="translate(0 97) rotate(-90)" fill="#850081">
    <path d="M 88.28727722167969 78 L 8.712726593017578 78 L 48.5 9.910438537597656 L 88.28727722167969 78 Z" stroke="none"/>
    <path d="M 48.5 19.82093048095703 L 17.42548370361328 73 L 79.57451629638672 73 L 48.5 19.82093048095703 M 48.5 0 L 97 83 L 0 83 L 48.5 0 Z" stroke="none" fill="#230101"/>
  </g>
</svg>
</li>
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