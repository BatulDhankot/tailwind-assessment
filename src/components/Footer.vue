<script setup lang="ts">
import { productLinks,companyLinks,supportLinks,contactInfo,IconClasses,iconPaths}  from '../../src/constant/common'
</script>

<template>
<!--Footer-->
<footer
  class="border-t text-center text-gray-500 lg:text-left divide-y">
  <!-- footer content -->
  <div class="container mx-auto px-4">
    <div class="mx-6 py-10 text-center md:text-left">
      <div class="grid-1 grid gap-8 md:grid-cols-2 lg:grid-cols-5">
        <div>
          <h6
            class="mb-4 flex items-center justify-center font-semibold uppercase md:justify-start">
            <img src="../assets/Travlog.svg" class="mr-3 h-6 sm:h-9" alt="logo" />
          </h6>
          <p>
           Lorem ipsum dolor sit amet, consectetur adipisicing
            elit.
          </p>
        </div>
        <div>    
          <h6
            class="mb-4 flex justify-center font-semibold uppercase md:justify-start text-black">
            Product
          </h6>
          <p v-for="link in productLinks" :key="link" class="mb-4">
      <a class="text-gray-500">{{ link }}</a>
    </p>
        </div>
        <div>
          <h6
            class="mb-4 flex justify-center font-semibold uppercase md:justify-start text-black">
            Company
          </h6>
          
          <p v-for="link in companyLinks" :key="link" class="mb-4">
      <a class="text-gray-500">{{ link }}</a>
    </p> 
        </div>

        <div>
          <h6
            class="mb-4 flex justify-center font-semibold uppercase md:justify-start text-black">
            Support
          </h6>
          <p v-for="link in supportLinks" :key="link" class="mb-4">
      <a class="text-gray-500">{{ link }}</a>
    </p> 
        </div>

        <div>
          <h6
            class="mb-4 flex justify-center font-semibold uppercase md:justify-start text-black">
            Contact
          </h6>
         
          <p  v-for="(contact, index) in contactInfo"  class="mb-4 flex items-center justify-center md:justify-start">
<svg :class="IconClasses[index]" xmlns="http://www.w3.org/2000/svg" width="28" height="28" viewBox="0 0 24 24" stroke-width="1.5" stroke="#597e8d" fill="none" stroke-linecap="round" stroke-linejoin="round">
  <path :d="iconPaths[index]" />
</svg>
           {{ contact }}
          </p>
        </div>
      </div>
    </div>
  </div>


  <!-- Copyrights -->
  <div class="p-6 text-justify">
    <span> Copyright © 2023</span>
  </div>
</footer>
</template>