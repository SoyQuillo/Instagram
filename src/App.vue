<script setup>

import { ref } from 'vue';

let notifications = ref(28)
let dislikes = ref(15)

function addLikes() {
  if(notifications.value = 28){
notifications.value++
dislikes.value == 15

}
}

function addDislikes(){
if(dislikes.value == 15){
  dislikes.value++
  notifications.value == 28
}
}
</script>

<template>
  
<div class="max-w-sm mx-auto shadow shadow-slate-400 mt-6 p-2">

  <div class="flex justify-between">

    <div class="text-xl font-bold">Historias</div>
    <div class="bg-blue-400 text-white w-12 h-6 rounded-md text-center">Todas</div>
  </div>
    <!-- CONTENEDOR CUATRO IMAGENES -->

    <div class="flex justify-between max-w-xs mx-auto mt-4">

      <div class="bg-[url('https://pbs.twimg.com/profile_images/1722501239450021888/oYy45eaU_400x400.jpg')] bg-cover h-16 w-16 border-2 border-blue-700 rounded-lg">
      </div>

      <div class="bg-[url('https://pbs.twimg.com/profile_images/1722501239450021888/oYy45eaU_400x400.jpg')] bg-cover h-16 w-16 border-2 border-blue-700 rounded-lg">
      </div>

      <div class="bg-[url('https://pbs.twimg.com/profile_images/1722501239450021888/oYy45eaU_400x400.jpg')] bg-cover h-16 w-16 border-2 border-blue-700 rounded-lg">
      </div>

      <div class="bg-[url('https://pbs.twimg.com/profile_images/1722501239450021888/oYy45eaU_400x400.jpg')] bg-cover h-16 w-16 border-2 border-blue-700 rounded-lg">
      </div>
      
    </div>

    <div class="flex justify-between max-w-xs mx-auto">

      <div  class="text-xs text-gray-400">Camila</div>
      <div class="text-xs text-gray-400">Maria Fer</div>
      <div class="text-xs text-gray-400">Señor x</div>
      <div class="text-xs text-gray-400">Juanca</div>

    </div>

    <div class="flex justify-between mt-6 p-2">

      <div class="flex gap-4">
        <div class="bg-[url('https://i.pinimg.com/736x/a4/91/33/a49133645c2475be6353ad1b7ae18c41.jpg')] bg-cover w-12 h-12 rounded-full"></div>
        <div>
          <h1>Marcos Perez</h1>
          <p>Hace 10 minutos</p>
        </div>
      </div>
      <div class="font-bold text-red-500">Reportar</div>
    </div>

    <div class="mt-4">
      <div class="bg-[url('https://www.santevet.es/uploads/images/es_ES/razas/labradorretrieversegurosantevet.jpeg')] bg-cover h-72 w-72 mx-auto rounded-md"></div>
    </div>

    <div class="flex gap-3 justify-center ">

      <div><svg @click="addLikes" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 hover:bg-red-500">
  <path stroke-linecap="round" stroke-linejoin="round" d="M21 8.25c0-2.485-2.099-4.5-4.688-4.5-1.935 0-3.597 1.126-4.312 2.733-.715-1.607-2.377-2.733-4.313-2.733C5.1 3.75 3 5.765 3 8.25c0 7.22 9 12 9 12s9-4.78 9-12z" />
</svg>
</div>

<div>
  <div>{{ notifications }} Me gusta</div>
</div>

<div>
  <svg @click="addDislikes" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6 hover:bg-blue-400">
  <path stroke-linecap="round" stroke-linejoin="round" d="M7.5 15h2.25m8.024-9.75c.011.05.028.1.052.148.591 1.2.924 2.55.924 3.977a8.96 8.96 0 01-.999 4.125m.023-8.25c-.076-.365.183-.75.575-.75h.908c.889 0 1.713.518 1.972 1.368.339 1.11.521 2.287.521 3.507 0 1.553-.295 3.036-.831 4.398C20.613 14.547 19.833 15 19 15h-1.053c-.472 0-.745-.556-.5-.96a8.95 8.95 0 00.303-.54m.023-8.25H16.48a4.5 4.5 0 01-1.423-.23l-3.114-1.04a4.5 4.5 0 00-1.423-.23H6.504c-.618 0-1.217.247-1.605.729A11.95 11.95 0 002.25 12c0 .434.023.863.068 1.285C2.427 14.306 3.346 15 4.372 15h3.126c.618 0 .991.724.725 1.282A7.471 7.471 0 007.5 19.5a2.25 2.25 0 002.25 2.25.75.75 0 00.75-.75v-.633c0-.573.11-1.14.322-1.672.304-.76.93-1.33 1.653-1.715a9.04 9.04 0 002.86-2.4c.498-.634 1.226-1.08 2.032-1.08h.384" />
</svg>
</div>

<div>
  <div>  <div>{{ dislikes }} No me gusta</div></div>
</div>


    </div>



    <div class="flex max-w-xs justify-between mx-auto mt-14 bg-gray-200 rounded-md h-12 text-center">

      <div class="w-8 h-8"><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M17.982 18.725A7.488 7.488 0 0012 15.75a7.488 7.488 0 00-5.982 2.975m11.963 0a9 9 0 10-11.963 0m11.963 0A8.966 8.966 0 0112 21a8.966 8.966 0 01-5.982-2.275M15 9.75a3 3 0 11-6 0 3 3 0 016 0z" />
</svg>
</div>
      <div><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
</svg>
</div>
      <div>
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 15.75l-2.489-2.489m0 0a3.375 3.375 0 10-4.773-4.773 3.375 3.375 0 004.774 4.774zM21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
</svg>
      </div>
    </div>
</div>
</template>

