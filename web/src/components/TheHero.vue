<template>
<div class="relative min-h-screen w-screen bg-slate-800">
 <div class="fixed top-0 left-0 right-0 flex flex-nowrap">
   <div class="relative">
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


  <nav class="flex absolute top-0 relative justify-start md:justify-end h-screen md:h-[5vh] md:w-1/4">
   <button class="absolute top-0 right-0 rounded-none h-[10vh] md:h-[5vh] z-50 bg-black w-1/4 md:w-0"></button>
   <ul class="absolute top-0 -right-1 z-40 md:z-0 flex flex-col h-full md:flex-row justify-center items-center py-2 px-3 bg-red-600 text-1xl font-bold">
       <li class="my-5 md:my-0 py-2 px-6 tracking-widest">HOME</li>
       <li class="my-5 md:my-0 py-2 px-6 tracking-widest">PROJECTS</li>
       <li class="my-5 md:my-0 py-2 px-6 tracking-widest">GITHUB</li>
     </ul>
     </nav> 
</div>
   
</div>
 <div class="flex items-center justify-center w-full h-screen">
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