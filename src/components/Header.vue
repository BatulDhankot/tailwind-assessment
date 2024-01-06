<script setup lang="ts">
import {ref } from 'vue'
import { menuItems }  from '../../src/constant/common'
const showMenu = ref(false)

</script>

<template>
  <div class="p-8">
    <!-- Header -->
    <header>
    <nav class="bg-white border-gray-200 px-4 lg:px-6 py-2.5">
        <div class="flex flex-wrap justify-between items-center mx-auto">
           <img src="src/assets/Travlog.svg" class="mr-3 h-6 sm:h-9" alt="logo" />
            <div class="flex items-center lg:order-2">
                <a href="#" class="text-gray-800  font-bold hover:text-white hover:bg-purple-800 focus:outline-none focus:ring-4 focus:ring-purple-300 
        rounded-full text-sm px-4 lg:px-5 py-2 lg:py-2.5 mr-2  ">Log in</a>
        <a href="#" class="text-white  font-bold hover:text-white bg-purple-800 hover:bg-purple-800 focus:outline-none focus:ring-4 shadow-lg shadow-purple-200
        rounded-full text-sm  px-4 lg:px-5 py-2 lg:py-2.5 mr-2">Sign Up</a>
                <button @click="showMenu = !showMenu" data-collapse-toggle="mobile-menu-2" type="button" class="inline-flex items-center p-2 ml-1 text-sm text-gray-500 rounded-lg lg:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200">
                    <span class="sr-only">Open main menu</span>
                    <svg class="w-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
                    <svg class="hidden w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
                </button>
            </div>
                <ul :class="showMenu ? 'flex absolute bg-white w-full' : 'hidden'" class=" flex flex-col mt-64 lg:bg-white md:bg-white lg:relative md:relative  font-medium lg:flex-row lg:space-x-8 lg:mt-0 
            space-y-4
            md:flex
            md:space-y-0
            md:flex-row
            md:items-center
            md:space-x-10
            md:mt-0" >
                  <li v-for="(HeaderItem, index) in menuItems" :key="index" class="text-sm font-bold text-gray-800 hover:text-indigo-700 text-center">
             {{HeaderItem}}
          </li>
         </ul>
        </div>
    </nav>
</header>

<!-- Banner Section -->
        <section class="px-8">
          <div class="lg:justify-items-start sm:justify-items-center lg:grid lg:grid-cols-2 md:grid md:grid-cols-2 gap-4 mt-14 ">

<div class="flex flex-col items-center text-center">
  <div>
    <!-- Button with text and icon -->
    <button type="button" class="border-gray-300 shadow-lg text-gray-800 font-bold hover:text-white hover:bg-purple-800 focus:outline-none 
    focus:ring-4 focus:ring-purple-300 rounded-full text-sm px-5 py-2.5 mb-2">
      <span class="flex justify-center items-center">
        <span class="mx-2">Explore the World! </span>
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-briefcase" width="28" height="28" viewBox="0 0 24 24" stroke-width="1.5" stroke="#fd0061" fill="none" stroke-linecap="round" stroke-linejoin="round">
  <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
  <path d="M3 7m0 2a2 2 0 0 1 2 -2h14a2 2 0 0 1 2 2v9a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2z" />
  <path d="M8 7v-2a2 2 0 0 1 2 -2h4a2 2 0 0 1 2 2v2" />
  <path d="M12 12l0 .01" />
  <path d="M3 13a20 20 0 0 0 18 0" />
</svg>
      </span>
    </button>
  </div>
  <div class="font-bold lg:text-7xl text-4xl mt-5">
    Travel <span class="text-pink-600">top </span>
    <div>
      <span class="text-pink-600"> destination</span>
    </div>
    of the world
  </div>
  <div class="mt-5">
    <div>where adventure meets comfort, we create</div>
    <div>unforgettable travel experiences</div>
  </div>
  <div class="flex flex-col md:flex-row gap-4 mt-5">

    <!-- Two buttons in a row/column -->
    <button type="button" class="bg-purple-800 border-gray-300 font-bold text-white hover:bg-purple-800 focus:outline-none 
    focus:ring-4 focus:ring-purple-300 rounded-full text-sm px-5 mb-auto py-4">Get Started</button>
    <button type="button" class="border first:font-bold text-gray-800 hover:text-white hover:bg-purple-800 focus:outline-none focus:ring-4
     focus:ring-purple-300 rounded-full text-sm px-5 py-2.5 mb-14">
      <span class="flex justify-center items-center">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-player-play" width="28" height="28" viewBox="0 0 24 24" stroke-width="1.5" stroke="#6f32be" fill="none" stroke-linecap="round" stroke-linejoin="round">
  <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
  <path d="M7 4v16l13 -8z" />
</svg>
        <span class="mx-2 font-bold">Watch demo</span>
      </span>
    </button>
  </div>
</div>

<!-- world Image section -->
<div>
  <div class="relative">
            <img
              src="src/assets/layer.svg"
              class="absolute scale-[1.32] top-12 right-6 lg:left-0 lg:w-[590px] md:left-0 md:w-[590px] sm:left-24 sm:w-[300px]"
              alt="layer"
            />
            
            <div class="bg-blue-500 lg:w-[600px] lg:h-[600px] md:w-[400px] md:h-[400px] sm:w-[300px] sm:h-[300px] sm:px-7 w-[200px] h-[200px] lg:rounded-full md:rounded-full sm:rounded-full rounded-full">
              <div class="w-full h-full z-500 flex justify-center item-center bg-no-repeat lg:left-0  sm:left-32 relative">
                <button class="bg-white z-10 left-36 xs:left-20 lg:left-80 bottom-5 lg:bottom-auto lg:top-1/2 lg:-translate-y-1/2 relative rounded-3xl shadow-lg  lg:w-30 h-14 lg:h-20 flex items-center justify-between mb-4 lg:mb-12 gap-2 lg:gap-3 shadow-gray-600/20 border-gray-100 text-theme-black whitespace-nowrap px-5 lg:px-7 hover:shadow-lg hover:shadow-theme-pink/50 hover:bg-theme-pink">
  <div>
    <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-broadcast" width="24" height="24" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffbf00" fill="none" stroke-linecap="round" stroke-linejoin="round">
      <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
      <path d="M18.364 19.364a9 9 0 1 0 -12.728 0" />
      <path d="M15.536 16.536a5 5 0 1 0 -7.072 0" />
      <path d="M12 13m-1 0a1 1 0 1 0 2 0a1 1 0 1 0 -2 0" />
    </svg>      
  </div>
  <p class="text-xs lg:text-2xl text-purple-700 font-bold lg:mb-2">
    5000+
    <span class="text-xxs lg:text-xs block lg:inline">Customer</span>
  </p>
</button>
                <img
                  src="src/assets/banner.svg"
                  class="absolute bottom-0 lg:self-end lg:bottom-auto lg:left-0 lg:h-auto"
                  alt=""
                 />
              </div>
              <button class="bg-white min-w-fit bottom-5 right-2 sm:right-20 lg:right-24 md:min-w-fit relative -top-10 lg:-top-40 rounded-3xl shadow-lg w-20 sm:w-30 h-10 sm:h-14 
              flex items-center justify-between mb-4 lg:mb-12 gap-2 sm:gap-3 shadow-gray-600/20 border-gray-100 text-theme-black whitespace-nowrap px-5 
              sm:px-7 hover:shadow-lg hover:shadow-theme-blue/50 hover:bg-theme-blue">
                <div>
                  <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-map-pin-filled" width="30" height="30" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffbf00" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M9 11a3 3 0 1 0 6 0a3 3 0 0 0 -6 0" />
                    <path d="M17.657 16.657l-4.243 4.243a2 2 0 0 1 -2.827 0l-4.244 -4.243a8 8 0 1 1 11.314 0z" />
                  </svg>
                </div>
                <span class="font-medium lg:inline"> Top Places</span>
              </button>
              <button class="bg-white bottom-28 lg:bottom-36 lg:left-80 lg:w-42 lg:h-14 left-1/2 relative rounded-3xl shadow-lg flex items-center justify-between mb-4 lg:mb-12 gap-3 shadow-gray-600/20 border-gray-100 text-theme-black whitespace-nowrap px-7 lg:px-8 hover:shadow-lg hover:shadow-theme-blue/50 hover:text-black hover:bg-theme-blue">
  <div>
    <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-map-pin-filled" width="30" height="30" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffbf00" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M9 11a3 3 0 1 0 6 0a3 3 0 0 0 -6 0" />
                    <path d="M17.657 16.657l-4.243 4.243a2 2 0 0 1 -2.827 0l-4.244 -4.243a8 8 0 1 1 11.314 0z" />
                  </svg>
  </div>
  <span class="font-medium hidden lg:inline">Top Hotels</span>
  <span class="font-medium lg:hidden">Hotels</span>
</button>

            </div>
          </div>
        </div>
</div>
        </section>
    </div>
</template>