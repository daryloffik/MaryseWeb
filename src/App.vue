
<script setup>

import Header from './components/Header.vue'
import Image from './components/Image.vue'
import about from './components/about.vue'
import work from './components/work.vue'
import contact from './components/contact.vue'

const Name= "Maryse ANIAMBOSSOU"
</script>

<template >

<Header :logo=Name >

</Header>
 <div class="flex flex-col mt-10 justify-center items-center ">
  <div class="lg:flex lg:flex-row lg:gap-10">
    <Image class="m-10">
  </Image>
  <div class="mt-5 m-5 ml-14 lg:ml-5 flex flex-col justify-center">
  
    <p class="lg:text-xl mt-5">Bonjour je suis Maryse,</p>
    <span class="text-3xl lg:text-5xl lg:max-w-[459px] text-slate-700 font-extrabold ">Juriste en droit des affaires et fiscalité </span>
    <p>Basé au Bénin</p>
    
  </div>
 
  </div>
 
  <about id="apropos"></about>
  <work id="work"></work>
  <contact id="contact"></contact>
 </div>
</template>

<style scoped>

</style>
