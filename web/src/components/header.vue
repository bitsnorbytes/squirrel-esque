 <template>
  <div class="bg-slate-800 fixed relative top-0 left-0 right-0 flex">

     <div class="flex justify-start w-full md:w-3/4 h-[10vh]">
     <ul class="flex items-center p-1 md:p-2 bg-red-600 text-2xl md:text-4xl font-bold">
       <li class="shadow-effect text-violet-900	 px-3 md:px-4 py-2">P</li>
       <li class="shadow-effect text-violet-900	 px-3 md:px-4 py-2">Y</li>
       <li class="shadow-effect text-violet-900	 px-3 md:px-4 py-2">S</li>
       <li class="shadow-effect text-violet-900	 px-3 md:px-4 py-2">L</li>
     </ul>
     <ul class="flex items-center ml-3 p-1 md:p-2 bg-red-600 text-2xl md:text-4xl font-bold h-[10vh]">
       <li class="shadow-effect text-violet-900	p-2">R</li>
       <li class="shadow-effect text-violet-900	p-2">E</li>
       <li class="shadow-effect text-violet-900	p-2">D</li>
     </ul>  

  </div>

  <button class="evp-mobile-nav-menu-toggle block md:hidden absolute top-0 right-0 w-20 aspect-square h-[10vh] z-50" :class="{ 'evp-mobile-nav-menu-toggle-open': ishideMenu,'evp-mobile-nav-menu-toggle-close': isShowMenu }" @click="toggleMenu"><span></span></button>
  <nav class="block flex fixed top-0 right-0 justify-start md:justify-end h-screen md:h-[10vh] md:w-1/4 z-40 md:translate-x-0 w-full ease-in-out duration-300" :class="{ 'translate-x-full':ishideMenu, 'translate-x-0': isShowMenu }">
   <ul class="absolute top-0 -right-1 z-40 md:z-0 flex flex-col h-full md:flex-row justify-center items-center py-2 px-3 bg-red-600 text-1xl font-bold">
       <li><router-link class="my-5 md:my-0 py-2 px-14 md:px-6 tracking-widest" to="/">HOME</router-link></li>
       <li><router-link class="my-5 md:my-0 py-2 px-14 md:px-6 tracking-widest" to="/projects">PROJECTS</router-link></li>
       <li><router-link class="my-5 md:my-0 py-2 px-14 md:px-6 tracking-widest" to="/contact">CONTACT</router-link></li>
     </ul>
     </nav> 
   
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
.shadow-effect {
   text-shadow: -4px 4px #fadbee,
   -3.75px 3.75px #fadbee,
   -3.5px 3.5px #fadbee,
   -3.25px 3.25px #fadbee,
   -3px 3px #fadbee,
   -2.75px 2.75px #fadbee,
   -2.5px 2.5px #fadbee,
   -2.25px 2.25px #fadbee,
   -2px 2px #fadbee,
   -1.75px 1.75px #fadbee,
   -1.5px 1.5px #fadbee,
   -1.25px 1.25px #fadbee,
   -1px 1px #fadbee,
   -.75px .75px #fadbee,
    -.5px .5px #fadbee,
     -.25px .25px #fadbee,
     -0px .0px #fadbee;
}
</style>